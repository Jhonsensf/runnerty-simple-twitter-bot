## Runnerty Demo - A simple runnerty twitter bot

This a [Runnerty](https://github.com/runnerty/runnerty) demo than builds a simple runnnerty bot.

It uses the `@runnerty-trigger-twitter` to listen to new followers to the user account. 

Everytime an user follows the account the trigger fires the chain sharing the data of the new follower. The chain has only two processes:

    - SEND_DIRECT_ES: It checks the language ot he new follower and if it is equal to 'es' The process sends a direct message to the new follower in Spanish
    - SEND_DIRECT_EN: It checks the language ot he new follower and if it is not equal to 'es' The process sends a direct message to the new follower in Spanish

This a simple example of the usage of the trigger and the executor but changing the params it's possible to add or change the funcionalities. Have a look at [trigger](https://www.npmjs.com/package/@runnerty/trigger-twitter) and [executor](https://www.npmjs.com/package/@runnerty/executor-twitter) documentation on npm to ***custom the chain***

## Usage
Clone the repo
```
git clone https://github.com/Jhonsensf/runnerty-simple-twitter-bot.git
```

Go to the directory  
```
cd runnerty-simple-twitter-bot
npm install
```

Run Runnerty
```
runnerty
```

###Expected result:

The chain will listen to new followers of the given Twitter accound and send them automatically a direct message.
