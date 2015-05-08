Giving Impact Campaign Boilerplate Theme for Statamic
=====================================================

## Overview

A Statamic starter theme to help jumpstart getting to know and creatively utilizing Giving Impact &trade; to create custom online fundraising solutions. The theme is designed to deliver a team-based fundraiser and to showcase the power of the combination of Giving Impact's dashboard, API, use of Stripe.com, and Statamic.

Giving Impact is online fundraising for Stripe, designed to unleash the creativity of designers and developers to deliver customized online donation experiences for Nonprofits.

For more about Giving Impact and to view our full documentation and learning reasources please visit [givingimpact.com](http://givingimpact.com)

### Theme Credits

**Developed By:** Minds On Design Lab - http://mod-lab.com
**Version:** 1.0
**Copyright:** Copyright &copy; 2010-2014 Minds On Design Lab
**License:** Licensed under the MIT license - Please refer to LICENSE

## Requirements

* [Statamic](http://statamic.com)
* [Statamic Giving Impact Add-on](https://github.com/Minds-On-Design-Lab/Statamic-Plugin-GivingImpact)
* A [Giving Impact](http://givingimpact.com) account.
    * Can use a developer sandbox account, please [contact Giving Impact to get one](http://givingimpact.com/contact)
    * Supports v2 of API
* Tested in Statamic 1.10.2

## Install

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

## Fundraiser Design

## Screencast

## Feedback
