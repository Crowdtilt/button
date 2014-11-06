#Tilt Button

## Allow users to create Tilt.com campaigns directly from your website.

### Demo:

[![](https://s3-us-west-2.amazonaws.com/tilt-button/split_with_tilt.png)](https://www.tilt.com/campaigns/new?collect=1&tilt=100&target=200&title=Split%20the%20cost%20with%20the%20Tilt%20button&description=Get%20started%20in%20minutes!%20Need%20help?%20We've%20got%20your%20back!%20support.api@tilt.com)

The result:    
![](https://s3-us-west-2.amazonaws.com/tilt-button/example_campaign.png)


### Use cases

* Added to your checkout confirmation page to split the cost of an item
* Added in your payment confirmation email to allow users to pool funds for an event or rental
* Added in your product flow to allow users to collect group funds for an event or experience

### Installation

Create a link with the following URL as the target:

```
https://www.tilt.com/campaigns/new?collect=1
&tilt=
&target=
&title=
&description=
```

Example: 

```
<a href="https://www.tilt.com/campaigns/new?collect=1&tilt=100&target=200&title=Split%20the%20cost%20with%20the%20Tilt%20button&description=get%20tilted">
Split the cost with Tilt
</a>
```

Arguments:

```&tilt=``` - the minimum amount before cards are charged ([learn more](https://us.support.tilt.com/hc/en-us/articles/200811869-What-s-a-tilt-amount-And-how-does-it-work-%20))    
```&target=``` - the ideal amount the campaign admin would like to collect    
```&title=``` - the title of the campaign    
```&description=``` - the description of the campaign


Optional:

```&contribution_type=preset``` - create a campaign that requires a preset, fixed contribution amount
```&incamount=``` - the fixed contribution amount required of contributors (can only be used when contribution_type=preset)    
```&maxquantity=``` - the maximum number of fixed-cost contributions that can be made (can only be used when contribution_type=preset)    
```&promotion_code=``` - pass through a promo code to waive [fees](https://www.tilt.com/learn/fees) (our default "collect money" option is always free)

### Advanced

#### Additional button assets

![Fund a cause with Tilt](https://s3-us-west-2.amazonaws.com/tilt-button/fund_a_cause.png)

![Collect money with Tilt](https://s3-us-west-2.amazonaws.com/tilt-button/collect_money.png)

#### Accessing campaign data

Campaign data in the format of a JSON array is can be accessed by appending ```/stats.json``` to any campaign URL.

Example:    

```
https://www.tilt.com/campaigns/save-the-toy-store/stats.json
```

#### Co-branded pages

Interested in having your brand's logo displayed on campaigns created through Tilt buttons on your site? Contact us at [support.api@tilt.com](support.api@tilt.com)

![ESPN + Tilt](https://s3-us-west-2.amazonaws.com/tilt-button/espn_tilt.png)

Want to see co-branded pages in action? Check out [reddit.tilt.com](https://reddit.tilt.com/campaigns/finding-a-dog-for-simon) and [espn.tilt.com](http://espn.tilt.com)

### Coming Soon

We're hard at work cooking up features to make starting Tilt campaigns from your website even better.

Here's a quick preview of things to come:

* Pass through a campaign image
* Fully branded creation flows
