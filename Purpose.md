# Dell HR Project

## Frontend
   - **Purpose**:
        - allow HR to view stats about external job portal
        - allow HR control syncing of job data to external job listing sites
   - **Tech**:
        - build on top of existing jobs.dell.com site
        - assuming they are using Angular, build on top of it
   - **Deployment**:
        - follow existing deployment practices

## Backend
   - **Purpose**:
        - handle the syncing from jobs.dell.com to external jobs site via API requests
        - handle monitoring of sync stats and statuses
   - **Tech**:
        - Java, Spring, Hibernate
        - SQL Server (depends on DB admins)
   - **Deployment**:
        - depends on what the company best practice is
        - Cloud Foundry


## Scripting
   - **Purpose**:
        - import existing jobs from external sites
        - compare it against jobs.dell.com jobs
        - update them and keep them in sync
            - jobs.dell.com
            - external sites
        - *no existing APIs for jobs data from external sites, have to scrape using web scraper*
   - **Tech**:
        - Python, SQLAlchemy
        - find a web scraper library