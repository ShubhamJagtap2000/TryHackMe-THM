# Task 6 - Maintaining Your System: Automation 

Users may want to schedule a certain action or task to take place after the system has `booted`. 

Take, for example, running commands, backing up files, or launching your favourite programs on, such as Spotify or Google Chrome.

We're going to be talking about the `cron` process, but more specifically, how we can interact with it via the use of `crontabs` . 

`Crontab` is one of the processes that is started during boot, which is responsible for facilitating and managing cron jobs.

![Screenshot (767)](https://user-images.githubusercontent.com/63872951/179571217-04a5bf65-995c-4a0b-aef5-69d504bc8569.png)

- A `crontab` is simply a special file with formatting that is recognised by the cron process to execute each line step-by-step. 
 
- Crontabs require `6` specific values:

|Value|	Description|
|--| --|
|MIN|	What minute to execute at|
|HOUR|	What hour to execute at|
|DOM|	What day of the month to execute at|
|MON|	What month of the year to execute at|
|DOW|	What day of the week to execute at|
|CMD|	The actual command that will be executed |


Let's use the example of backing up files. 

You may wish to backup `cmnatic`'s  `Documents` every `12` hours. 

- We would use the following formatting: 

`0 *12 * * * cp -R /home/cmnatic/Documents /var/backups/`

- An interesting feature of `crontabs` is that these also support the `wildcard or asterisk (*)`. 

- If we do not wish to provide a value for that specific field, i.e. we don't care what month, day, or year it is executed -- only that it is executed every `12` hours, we simply just place an `asterisk`.

- This can be confusing to begin with, which is why there are some great resources such as the online [Crontab Generator](https://crontab-generator.org/) that allows you to use a friendly application to generate your formatting for you! As well as the site [Cron Guru!](https://crontab.guru/).

- Crontabs can be edited by using `crontab -e`, where you can select an editor (such as `Nano`) to edit your crontab.


![Screenshot (768)](https://user-images.githubusercontent.com/63872951/179572292-fc655ebb-7cf1-414b-aa14-ff76dec2c927.png)

![Screenshot (769)](https://user-images.githubusercontent.com/63872951/179572445-7b99faa1-b462-4cf8-9c5e-12ebdb12c86b.png)

# Answer the questions below

1. When will the crontab on the deployed instance (MACHINE_IP) run?
```
@reboot
```








