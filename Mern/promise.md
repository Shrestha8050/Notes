# Promise

_Promise is an object which represent future result value._
The Promise object represents the eventual completion (or failure) of anasynchronous operation (operation that takes time ) and its resulting value.
In promise, asynchronous methods doesnot return the value directly but it returns a promise to supply the value at some point in the future.

### A Promise is in one of these states:

        1. pending: initial state, neither fulfilled nor rejected.
        2. fulfilled: meaning that the operation was completed successfully.
        3. rejected: meaning that the operation failed.

### Promise Methods

        The methods are used to associate(connect) further action with a promise after becomes settled.
        These methods also return a newly generated promise object, which can optionally be used for Promise chaining.

        There are three methods used in Promise
            1. Promise.then()
                -Used to handle both success and failure (Recomended to use for success )
            2. Promise.catch()
                - Used to handle failure only
            3. Promise.finally()
                - Executed once promise is settled

### Syntax of Promise

        const myPromise = new Promise(function(success,failure){
            //1st argument is placeholder for success callback
            //2nd arguement is placeholder for failure callback
            //if success runs success()
            //if failure runs failure()

        })

        myPromise
            .then(handleFulfilled)
            .catch(handleRejectedA)
            .finally(completed Statement)


        Example:--

        const mypromise =  new Promise(function(resolve,reject){
            //For delaying the data delivery
            setTimeout(function(){
                resolve()
                //reject()
            },2000);
        })

        mypromise
            .then(function(){
                console.log('Success');
            })
            .catch(function(){
                console.log('Failure');
            })
            .finally(function(){
                console.log('After settled Part');
            })

### Nested Promise Syntax

            const myPromise = new Promise(function(success,failure){

            //if success runs success()
            //if failure runs failure()

        })

        myPromise
            .then(handleFulfilled)
            .then(handleFulfilled1)
            .then(handleFulfilled2)
            .catch(handleRejectedA)
            .finally(completed Statement)


          Example:--

        const mypromise =  new Promise(function(resolve,reject){
            //For delaying the data delivery
            setTimeout(function(){
                resolve()
                //reject()
            },2000);
        })

        mypromise
            .then(function(){
                console.log('Success');
                return Promise object
            })
            .catch(function(){

                // It catches the passed Promise object from above then method
                console.log('Failure');
            })
            .finally(function(){
                console.log('After settled Part');
            })
