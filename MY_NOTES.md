# Notes made during project implementation
**During every tutorial project, I make notes on what I had to do to achieve the goal. These notes are stored here.**

The instructions are somewhat outdated: ECS now has the express service creation which automatically creates a Fargate instance with load balancer; an EC2 instance does not have to be added manually. I managed to repeat the tutorial twice, once with a EC2 instance and once with the newer method(Fargate). The next issues happened with a Fargate instance only.
This website is assigned the port 8000 instead of usual 8080, this was important to notice and change manually in Express service settings.
Also the website has no default response ("/" address) which makes the default health check of the service fail, the check's address also had to be changed manually to "/hello/".
