Giving Impact Campaign Boilerplate Theme for Statamic
=====================================================

## Overview

A Statamic starter theme to help jumpstart getting to know and creatively utilizing Giving Impact &trade; to create custom online fundraising solutions. The theme is designed to deliver a team or peer to peer fundraiser and to showcase the power of the combination of Giving Impact's dashboard, API, use of Stripe.com, and Statamic.

Giving Impact is online fundraising for Stripe, designed to unleash the creativity of designers and developers to deliver customized online donation experiences for Nonprofits.

For more about Giving Impact and to view our full documentation and learning resources please visit [givingimpact.com](http://givingimpact.com).

### Theme Credits

**Developed By:** Minds On Design Lab - http://mod-lab.com
**Version:** 1.0
**Copyright:** Copyright &copy; 2010-2015 Minds On Design Lab
**License:** Licensed under the MIT license - Please refer to LICENSE

## Requirements

* [Statamic](http://statamic.com)
* [Statamic Giving Impact Plugin](https://github.com/Minds-On-Design-Lab/Statamic-Plugin-GivingImpact)
* A [Giving Impact](http://givingimpact.com) account.
    * Can use a developer sandbox account, please [contact Giving Impact to get one](http://givingimpact.com/contact)
    * Supports v2 of API
* Tested in Statamic 1.10.2


## Theme Details & Fundraiser Design

The following are some key details about this theme, it's use of Statamic, and Giving Impact.

### About the Fundraiser

![Homepage - Screen](/readme-imgs/home_w_data.png)

This theme is a boilerplate, a lightweight working but ready to be designed and tweaked to your unique online fundraising needs.

It's designed to harness the power of Giving Impact's online fundraising API (that works with Stripe.com) and the awesome speed and flexibility of Statamic's CMS platform to allow you to set up the core of team/advocate campaign site in minutes.

Key Details

* You can donate to the campaign as a whole or member created "teams".
* "Team" pages can be created from the site by site members.
  * Creates a "Giving Opportunity" within the site's camapign in Giving Impact with the member associated with it via email.
* Donations forms are fully integrated, seamlessly in the site.
  * Using Giving Impact's hosted dashboard, campaign managers can enable donation levels, automated email receipts, custom donation fields to capture data from donors and have all these functionality reflected in the donation forms powered by this theme.

* Fully seamless use of Giving Impact's online fundraising API for Stripe.com. Donors and campaign users will only interact with the site and brand it would showcase.

### Theme Details

* The theme uses [Skeleton](http://getskeleton.com/) which is a very lightweight responsive front end boilerplate.
* The theme uses Statamic's Member functionality. In order to create a team/fundraiser page, you must register to create a member account.

## Statamic Install

To install the theme follow the instructions below.

1. [Install Statamic:](http://statamic.com/learn/digging-in/installing) **Don't forget to set up your .htaccess file**.
2. Copy the campaign-boilerplate theme folder to your _themes folder.
3. Download and install the [Statamic Giving Impact Plugin](https://github.com/Minds-On-Design-Lab/Statamic-Plugin-GivingImpact) Plugin
 * You will need a Giving Impact account and API keys. To Request a free developer account please [contact Giving Impact to request one](http://givingimpact.com/contact)
5. This theme does require specific content. You will need to delete the contents of your existing _content folder and copy the files and folders from the this theme's _content folder.
6. In your Statamic install go to `_config` settings YAML file and change the `_theme` name to `campaign-boilerplate`

**IMPORTANT - Security - If using this theme in production with a paying Giving Impact subscription, the website must be hosted with SSL**

### Custom Routes

Add the following to your `_config\routes.yaml` file.

```
/teams/detail:
  template: team/detail
/teams/{token}/detail:
  template: team/detail
/teams/{token}/donate:
  template: team/donate
/teams/{token}/thanks:
  template: team/thanks
```

## Giving Impact Setup

1. First you need to have a Giving Impact account, paid or developer. Details shared above.
2. Log in and get your account connected to Stripe. [Check out the docs](http://givingimpact.com/docs/developer-account) about the developer account to help.
3. Create the Campaign you want to use for this site.

Make sure you set the Campaign to use Giving Opportunities as pictured below and then feel free to explore the other settings and how they work with the site.

![Giving Impact - Screen](/readme-imgs/gi_camp_setup.png)

4. Finally you need to get your Campaign's token and add that to the theme.yaml file in the `_themes/campaign-boilerplate` folder.

You can find the token from the Giving Impact dashboard as highlighted below.
![Giving Impact - Screen](/readme-imgs/gi_token.png)

5. Okay time to explore and see what Giving Impact and this theme can do. Then go make them your own from here.

## Screencast

Needed and Coming Soon - The plan

## Feedback

Did you try it out? Having trouble? We'd like to know. Post a Github issue or reach out to us on [Twitter](https://twitter.com/mindsondesign)
