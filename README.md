Scheduling your tasks using Job Scheduler API:      

JobScheduler api introduced in API21 to perform background tasks.  

This API allows you to run scheduled service and the android system will batch all the services from different applications 
and run them together in some particular timeframe. The reason behind this is to reduce the amount of time your phone’s CPU 
and radio wakes up by batching the tasks together. This will consume less battery and maintains system health.     


What if your application has minSdkVersion &lt; 21?
In this situation the official way to schedule the job is to use Firebase Job Dispatcher. 
Firebase Job Dispatcher is supported to all the way down upto API9.
