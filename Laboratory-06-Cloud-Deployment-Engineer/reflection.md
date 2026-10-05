# Mission Reflection

Completing this laboratory activity helped me understand how Docker Compose makes the work of a cloud engineer easier and more organized. Instead of manually typing separate commands for every container, I was able to define the entire application setup inside a single `docker-compose.yml` file. This makes the deployment easier to repeat, manage, and troubleshoot because the configuration is already documented as code.

I also learned that YAML formatting is very important. An indentation error, such as using a tab instead of spaces or placing a line at the wrong level, can cause Docker Compose to fail when reading the file. This showed me that even small formatting mistakes can affect the deployment of an entire application.

Environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, `MYSQL_USER`, and `MYSQL_HOST` were used to provide the containers with the configuration they needed. These variables allowed the Nextcloud application to know which database to use and how to connect to the MariaDB service without manually configuring everything after the containers started.

Deploying Nextcloud and MariaDB using only a few commands was satisfying because it showed how quickly a functional multi-container cloud application can be created. Before this activity, I thought deploying an application with a separate database would require many complicated steps. Docker Compose made the process much simpler.

Since Mission 1, my understanding of cloud computing has improved significantly. I now understand that cloud computing is not only about storing files online. It also involves virtualization, containers, networking, storage, databases, automation, and Infrastructure as Code. This laboratory helped me see how these concepts work together when deploying a real application.
