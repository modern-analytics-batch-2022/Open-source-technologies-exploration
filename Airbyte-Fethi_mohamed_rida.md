
<p align="center">
    <img width="600" height="100" src="https://user-images.githubusercontent.com/64019836/154453227-1b6b047e-93c4-4be5-81c0-ee745fc72500.png"> 
</p>

## :point_right: _Description_
Airbyte is an open-source data integration platform that syncs data from  applications, APIs, and databases to warehouses. Airbyte’s modular architecture and open-source nature let's data engineering teams handle everything from one single platform.
<p align="center">
    <img width="600" height="300" src="https://user-images.githubusercontent.com/64019836/154456167-b6997c43-bad5-477f-800e-8614c43c333b.png"> 
</p>

## :point_right: General information:

- #### Creation year: January 2020
- #### Website:
                  https://airbyte.com/
- #### Github repo:
                  https://github.com/airbytehq/airbyte
- #### Community channel
     > :globe_with_meridians: Twitter : https://twitter.com/airbytehq <br>
     > :globe_with_meridians:Linkedin : https://www.linkedin.com/company/airbytehq/ <br>
     >:globe_with_meridians:Facebook : https://www.facebook.com/AirbyteHQ  <br>
     >:globe_with_meridians:Slack : https://airbytehq.slack.com/  <br>
     >:globe_with_meridians:Carrer : https://jobs.lever.co/airbyte  <br>
     >:globe_with_meridians:YOUTUBE : https://www.youtube.com/channel/UCQ_JWEFzs1_INqdhIO3kmrw  <br>
     >:globe_with_meridians:Discourse :https://discuss.airbyte.io/  <br>
- #### Community size:
 
 <p align="center">
    <img width="700" height="100" src="https://user-images.githubusercontent.com/64019836/154460704-2221751c-0599-4261-b68b-1b1133a74902.png"> 
</p>

- #### Founders:
 <p align="center">
    <img width="700" height="230" src="https://user-images.githubusercontent.com/64019836/154452128-c1844426-d1d4-405a-82e5-106622acec34.png"> 
</p>

<br>
Tricot, former Director of Engineering and Head of Integrations at Liveramp and RideOS, founded Airbyte with John Lafleur. Lafleur is described as a serial entrepreneur of B2B development and technology tools.
  
## :point_right: Main capabilities:

- **Built for extensibility:** Adapt an existing connector to your needs or build a new one with ease.
- **Optional normalized schemas:** Entirely customizable, start with raw data or from some suggestion of normalized data.
- **Full-grade scheduler:** Automate your replications with the frequency you need.
- **Real-time monitoring:** We log all errors in full detail to help you understand.
- **Incremental updates:** Automated replications are based on incremental updates to reduce your data transfer costs.
- **Manual full refresh:** Sometimes, you need to re-sync all your data to start again.
- **Debugging autonomy:** Modify and debug pipelines as you see fit, without waiting.
## :point_right: Available connectors / integrations

Airbyte uses a grading system for connectors to help users understand what to expect from a connector. There are three grades, explained below:
- **Certified:** This connector has been proven to be robust via usage by a large number of users and extensive testing.
This connector has been proven to be robust via usage by a large number of users and extensive testing.
- **Beta:** While this connector is well tested and is expected to work a majority of the time, it was released recently. There may be some unhandled edge cases but Airbyte will provide very quick turnaround for support on any issues (we'll publish our target KPIs for support turnaround very soon). All beta connectors will make their way to certified status after enough field testing.
While this connector is well tested and is expected to work a majority of the time, it was released recently. There may be some unhandled edge cases but Airbyte will provide very quick turnaround for support on any issues (we'll publish our target KPIs for support turnaround very soon). All beta connectors will make their way to certified status after enough field testing.
- **Alpha:** This connector is either not sufficiently tested, has extremely limited functionality (e.g: created as an example connector), or for any other reason may not be very mature
<p align="center">
    <img width="500"  src="https://user-images.githubusercontent.com/64019836/154476739-a0a6adc3-5447-48ac-afe7-c1c1d6092eec.png"> 
</p>
 
## :point_right: Ways to deploy it :

## On-prem
In an on-premises environment, resources are deployed in-house and within an enterprise’s IT infrastructure. An enterprise is responsible for maintaining the solution and all its related processes.
 - ###  Local Deployment:
    - Install Docker on your workstation
    - After Docker is installed, you can immediately get started locally by running:
        ```sh
           git clone https://github.com/airbytehq/airbyte.git
           cd airbyte
           docker-compose up
        ```
    - In your browser, just visit: http://localhost:8000 
## PaaS / SaaS
 **PaaS:** Platform as a service (PaaS) is a cloud computing model where a third-party provider delivers hardware and software tools to users over the internet. <br>
 **SaaS:** Software-as-a-Service(SaaS) refers to the installation and delivery of software as a service, as opposed to the traditional on premise model of software deployment
 - ### On AWS (EC2):
     is a service offered by Amazon allowing third parties to rent servers on which to run their own web applications. EC2 enables scalable deployment of applications by providing a web interface through which a customer can create virtual machines, i.e. instances of the server, on which the customer can load any software of their choice.
 - ### On Kubernetes:
    is an open-source system that aims to provide a "platform to automate the deployment, scaling, and implementation of application containers on server clusters"3. It works with a variety of containerization technologies, and is often used with Docker. It was originally designed by Google and then donated to the Cloud Native Computing Foundation.
 - ### On Azure(VM):
    Azure Virtual Machines (VM) is one of several types of on-demand, scalable computing resources that Azure offers.
    >1.Launch Azure Cloud Shell <br>
    >2.Create a new virtual machine <br>
    >3.Install environment <br>
    >4.Install and Start Airbyte <br>

- ### On Plural    
   Plural is a unified application deployment platform that makes it easy to run open-source software on Kubernetes. It aims to make applications as portable as possible, without sacrificing the ability for the users to own the applications they desire to use.
     >  1.First, create an account on https://app.plural.sh <br>
     >  2.Install the Plural CLI <br>
     >  3.Installing Airbyte:To install Airbyte on your Plural repo, simply run: <br>
                 ```sh
                   plural bundle install airbyte airbyte-aws
                 ```           
    > 4.After this, run: <br>
               ```sh
                plural build 
                ```
                <br>
                ```sh
                plural deploy --commit "deploying airbyte" 
              ``` 
              <br>
    >  5.Adding the Plural Console: <br>
             ```sh
                 plural bundle install console console-aws
              ```
              <br>
              ```sh
                 plural build 
              ```
              <br>
              ```sh
                 plural deploy --commit "deploying the console too" 
             ```

## :point_right: Reviews  
### :+1: Good reviews:
Airbyte’s core value proposition is centered around three factors: portability, accuracy, and security.
- **Portability**, or the ability to easily retrieve data, comes first. That's because accuracy only comes into play once data is readily available.
- After a business uses Airbyte to import data, the question then shifts into the **accuracy** of their ported data. As it relates to **accuracy**, Airbyte maintains strict rules around how their team manages schema changes and how they ensure assets are valid. 
- The final piece is **security**, which boils down to data warehouses and the intelligence Airbyte builds on top of their own pipes. Michel points out that the Airbyte team focuses a ton of time and energy on ensuring that data can safely move from any source to the final warehouse.
### :thumbsdown: Bad reviews:
The downsides of full containerization are the inherent performance costs and the added steps when modifying or building new connectors.
## :point_right: Roadmap  
- **Coming within a few days**: Check out our Roadmap for Core and our Roadmap for Connectors on GitHub. You'll see the features we're currently working on or about to. You may also give us insights, by adding your own issues and voting for specific features / integrations.
- **Coming within a few weeks / months**: We understand that we're not "production-ready" for a lot of companies yet. In the end, we just got started in July 2020, so we're at the beginning of the journey. Here is a highlight of the main features we are planning on releasing in the next few months:
- **Coming within a few quarters/years:** We also wanted to share with you how we think about the high-level roadmap over the next few months and years. We foresee several high-level phases that we will try to share here.

