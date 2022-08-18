# Product Requirements Document
## Summary

During the pandemic, I watched many people receive thousands of dollars in donations for essentially being themselves. The donees had shelter, food, water, and clothing to say the least. The goal of QRCodes2ComeHome is to enable the less fortunate with the means to accept digital transactions in a cost-effective manner with little to no cost on behalf of the homeless. 

If a person becomes homeless they are immediately cut off from the basic services they need to recover. The ability to apply for jobs, receive benefits, open a bank account, receive post: all are placed out of reach at the point they are needed most. Those who might have otherwise got back on their feet with a little early support are instead left to become entrenched in the situation and develop more complex and care-intensive needs over time.

While there are shelters, I personally have witnessed dozens of homeless on street corners or at the end of a bridge holding a piece of cardboard with cries for help such as "Need Help", "Down on their Luck", or "Will work for food". QRCodes2ComeHome believes in the intrisic good of humanity, in granting the chance to make a change for the better, and having a real impact on the everyday world you experience. This charity is not "I’m donating money in another country and running in circles to feel like I’ve done something to feel and aid the suffering of others in a place I'll never know and to people I'll never meet. This is, "I saw a human in need, and I reached out right then and there to make a knowable diffence in their life in my community. I gave them hope today for a brighter future tomorrow."

This document summarizes QRCodes2ComeHome. The charity is fundamentally comprised of a physical address, a cell phone, a reloadable debit card, and a PayPal account. By demonstrating how a person can setup a paypal account at a library using this charity's address and donated phone number, a QR code can be printed to accept donations for change. Donors can then scan the QR code to make instant donations to the individual by simply pointing their phone's camera at the code and choosing their means of payment. The donee recipient would then transfer the donation to the reloadable card to pay for the goods and services of daily living (food, clothing, shelter). 

Ultimately, the aim is to create a website which will provide social services to the homeless, log short and long term goals, provide instant feedback on the use of the donation to the donor through notifications, create a record of immutable transactions, and provide cards and accounts that are not reliant on PayPal or reloadable Visa debit cards. For the time being, QRCodes2ComeHome will focus on the fundamentals for a proof-of-concept and minimum-viable-product.

This document aims to identify the key features of the application and app to ensure each of these are delivered at launch.
1. [Objective](#objective)
2. [Release](#release)
3. [Features](#features)
4. [User flow and design](#user-flow-and-design)

## Objective
### Vision
A piece of cardboard with a QR code on it that can accept payments, a blog with instructions on how to operate, and a homeless person with a full stomach.

### Goals
Elevate the standards of living for the homeless by providing a method and means to eventually afford a common standard of living (food, clothing, shelter, healthcare, employment).

### Initiatives
- Provide a useable physical address to create a payment account with.
- Provide a cell phone number to create a Paypal account with. 
- Provide a reloadable debit card with which to buy goods and services. 
- Provide a way for the homeless to operate these services autonomously. (blog) 
- Donate to the homeless.

### Persona(s)
The homeless and citizens willing and able to make a donation.

## Release
### Release
QRCodes2ComeHome 1.0

### Date
12/31/2022

### Initiative
Launch the website and test the full lifecycle of the donation process for public trials before a full launch

### Initiatives
- Prototype Version 
- Contracts and Legal 
- Registration of non-profit
- Alpha Testing (solo)
- Beta Testing (with another)
- Launch (find customer)
- Delta Testing (iterate on feedback)

### Features
- cloud hosting
- physical phone
- paypal account
- cloudfront domain routing
- a domain
- https security on the endpoint
- a debit card
- non-profit registration

### Dependencies
- AWS
- Google Domains
- Angular/Vue Javascript
- API for message
- Legalzoom or sba for registration of charity (Legal Team)
- a customer
- a donor
- Kickstarter for funding
- earth class mail for an address 
- a visa reloadable debit card
- a phone for non-VoiP authentication
- a library
- change to print a qr code
- cardboard


## Features
### Feature
cloud hosting

### Description
Cloud hosting allows the blog of instructions to be hosted and available to the public at any time day or night.

### Purpose
Allows for accessiblity of information. If an email service or message service is implemented then it is a point of contact as well.

### User Problem
People may run into issues with the account and become unable to use this service. In order to reach the most people, a site will be hosted on the cloud to provide feedback, retention, and instructions on the process. 

### User Value
The user can have access to the internet through a library. 

### Assumptions
The users have access to a library, the necessary information to obtain a library card, and understand how to read and use the internet. 

### Not doing
Not providing on call or 24/7 customer support. 

### Acceptance criteria
A blog is acessible from a public library. 

### Feature
physical phone

### Description
A cheap $20 "burner" walmart non-Voip phone.

### Purpose
To create and authenticate a paypal account.

### User Problem
The customer may not have a phone nor the means for a monthly payment

### User Value
The customer can create a PayPal account to generate QR codes, accept donations, and transfer payments.

### Assumptions
The customer does not own a phone. The PayPal account does not require the use of a phone after account creation. 

### Not doing
Not providing a phone or phone service. Just setting up the account.

### Acceptance criteria
A new phone is used to create a paypal account.

### Feature
paypal account

### Description
A PayPal Account (non-business)

### Purpose
To generate QR codes, accept donations, and transfer donations to a reloadable debit card for use. 

### User Problem
The customer does not have a bank account.

### User Value
The customer can accept mobile payments via QR code. 

### Assumptions
The customer knows PI information to make an account, has the ability to use a computer, and access to a library computer. 
The customer does not have a drug or alcohol addiction, and uses the money responsibly for basic necessities so they are no longer homeless and no longer need this service. The customer is not a criminal, and does not possess criminal or evil intent.

### Not doing
Not allowing the account to be used for alcohol, weapons, drugs, sex trafficking, or any other nefarious or unhealthy activity.

### Acceptance criteria
The customer has a PayPal account registered in their name.

### Feature
cloudfront domain routing

### Description
Routing for a vanity URL.

### Purpose
Routes a vanity url to a server that hosts a blog.

### User Problem
A non-vanity url will need to be routed to a domain, and without domain routing, the blog instructions will not be easy to find. 

### User Value
The customer will be able to navigate to a blog for instructions and feedback.

### Assumptions
The users have access to a library, the necessary information to obtain a library card, and understand how to read and use the internet. 

### Not doing
Not paying for cloud hosting if out of budget (will use a github pages instead with an email listed to accept feedback; will help the customer make an email if needed)

### Acceptance criteria
The website is routed successfully to the domain and is navigable from a public library.

### Feature
a domain name

### Description
A listed internet domain name.

### Purpose
Allows the advertisement of the charity, and gives the customer a place to go to find instructions without memorizing a strange url.

### User Problem
The user will need instructions or a means to provide feedback or request assistance. The domain will be an easily rememberable means for a central source of information

### User Value
The user can navigate to a website and advertise the service to others. 

### Assumptions
The users have access to a library, the necessary information to obtain a library card, and understand how to read and use the internet. 

### Not doing
Not running a website that is out-of-budget or too costly.

### Acceptance criteria
a domain name is purchased with the value "QRCodes2ComeHome". Any endpoint will do.

### Feature
https security on the endpoint


### Description
HTTPS is added to the blog of the website

### Purpose
To allow the site to be safe and accessible to the public. 

### User Problem
The user may not be able to visit non-https sites from a public computer. 

### User Value
The user and library will be ensured that their data and network is safe. 

### Assumptions
The library can navigate to the site.

### Not doing
Not performing extensive or redundant security (not accepting credit card or PI online)

### Acceptance criteria
https is added to the domain.


### Feature
a debit card

### Description
A visa reloadable debit card.

### Purpose
To be used to buy goods in a store.

### User Problem
User does not have a bank account or access to money or a job. Everything has to be bartered, begged for, or paid with cash. Physical transactions have a risk of spreading diseases and viruses such as Covid-19.

### User Value
The user will be able to buy physical goods from a store.

### Assumptions
The user is fiscally responsible enough not to abuse the card. Having the card does not make the customer a target. The customer is honest. The customer does not lose the card. The customer does not use the card for evil, destructive, or illegal purchases. The customer does not sell the card.

### Not doing
Not buying a replacement card.

### Acceptance criteria
A reloadable visa card is purchased and money is loaded onto the card from the PayPal account.

### Feature
non-profit registration

### Description
Legal registration of the charity.

### Purpose
Will grant authenticity in the acts and services of QRCodes2ComeHome. Will enable tax exemption status and the opportunities to receive grants and other funding. Will enable the use of a bank account for the charity. Will enable the use of a physical address to lend to customers to create PayPal accounts.

### User Problem
The charity needs to be funded in some way, and the insterests of those involved must be protected and insured against crime and evil activities.

### User Value
The charity becomes an official organization, will be recognized, can receive tax exemption status and the opportunities to receive grants and other funding. Can lend addresses to customers for PayPal account creation. 

### Assumptions
The registration is not too expensive to maintain. Funding the charity through registration will outweight the costs of registration. 

### Not doing
Creating a small business or a for profit. Not creating a shell corp. Not using the charity for anything but the purpose of the charity as stated in this PRD.

### Acceptance criteria
A charity is successfully registered through sba.gov or LegalZoom.

