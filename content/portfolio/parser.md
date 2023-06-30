title: Data Scraping
description: application for automatic data scraping from websites with visualization
category: Selenium, PostgreSQL, Plotly, Docker
libraries: Selenium, BeautifulSoup, Dash
icon: bx bxs-bug
info: screenshot
link: "/static/img/parser_all.png"
sort: 5

###DESCRIPTION

Application for collecting data from various websites. In this implementation, it is configured for regular parsing of open vacancies in a certain category on the leading recruiting platform in Ukraine.

With a certain frequency, open vacancies on the platform are checked and all new ones are taken.

A random User-agent is used to protect against blocking.

All received data is added to the PostgreSQL database. A simple visual analytics on the Dash framework has also been added. Analytics can be complicated, but this was not the goal in this case.
When certain events are triggered, the Telegram bot sends an alert.

Optionally, the application can be deployed in Docker containers. This case uses 3 related docker containers.