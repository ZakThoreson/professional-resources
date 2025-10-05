# Notes for completeing the Cloud Resume Challenge  
This page serves as my notes on an abrigded approach to building a website to host my resume. Inspired by some reddit posts and the Cloud Resume Challenege, the goal is to get better at CI/CD, coding, and cloud architecture. 

# In Progress
* Develop a Huge Website
  * Deploy Locally
  * Migrate content from Thoreson Consulting
* Standardize resume for website consumption

# Goals 
* Use Terraform + Ansible to configure a Digital Ocean Droplet to host my website
* Configured host will leverage a website publicly hosted on my GitHub built by Hugo
* Include a CI/CD to push updates and deployments via a Dev & Prod environment
* Build analytics, logging, and tracking for analytics
* Write up on lessons learned / how I did it
* Implement security best practices and reporting

# Notes
* Plan to run the website via Digital Ocean Droplet
* Generate basic website code via Hugo
* Integrate CI/CD capabilities with Git
  * Add security scans (Chekov / Prowler / Trivy?)
  * The IaC component will be hosted internally (Gitea?) https://about.gitea.com/
  * Setting up Gitea Actions
    * https://docs.gitea.com/usage/actions/design
    * https://docs.gitea.com/usage/actions/act-runner
* Add counter / form submission
  * https://termly.io/resources/articles/website-tracking/ 
  * Ideas: Vistors by country, page popularity, re-directs? 
* Links / Blog Posts -> Medium + Thoreson Consulting old content

## Websites: 
* https://cloudresumechallenge.dev/
* https://gohugo.io

## References: 
* https://www.reddit.com/r/devops/comments/xd3wdl/comment/ioabi23/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button
* https://docs.netlify.com/get-started/
* https://www.netlify.com/blog/guide-to-ci-cd-automation-using-webhooks/#:~:text=At%20Netlify%2C%20we%20offer%20an,a%20robust%20CI%2FCD%20pipeline.
