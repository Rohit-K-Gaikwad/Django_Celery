### The architecture of Celery consists of the following components:
- **Task producers:** These are the components that generate tasks and submit them to the task queue. They can be Django views, command-line scripts, or any other code that needs to run a task asynchronously.
- **Message broker:** This is a message queue service that is responsible for storing the tasks until they are ready to be executed. Some popular message brokers include RabbitMQ and Redis.
- **Task consumers:** These are the components that listen for tasks in the message queue and execute them. They can be multiple worker processes running on different machines.
- **Result backend:** This is a database or message queue that is used to store the results of the tasks. The resulting backend is optional, but it can be used to retrieve the results of the tasks after they have been executed.

![celery architecture](https://github.com/Rohit-K-Gaikwad/Django_Celery/blob/main/static/Celery%20arch.png)
