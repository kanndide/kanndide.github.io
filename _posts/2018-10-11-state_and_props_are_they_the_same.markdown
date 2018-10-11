---
layout: post
title:      "State and Props? Are they the same? "
date:       2018-10-11 17:26:24 +0000
permalink:  state_and_props_are_they_the_same
---


No. Article finished. Whew. Good job, Larry! Just kidding.  

I'm Larry, in case you were wondering. If not, now you know anyway. So, state and props. Let me first start by explaining that a `class` defined with `React.Component`  and a regular JavaScript function are very similar. One of the differences with these React components is state and props.  

State is a components local state. It only affects the particular component it is defined in. Props (like properties, shout out Flatiron) is more of a set property. It is very similary to passing in arguments for a regular function. 

``` 
const sayHello = (hello) => {
      console.log(`${hello}`)
}
```  

The above example is just a function with an argument passed through it but it is similar to how props work with react components.  
With state, they are set locally within a class.

```
class iAmAComponent extends React.Component {
    state = {
		    count: 0
		}
		
		render() {
		    return(
				    <p>{this.state.count}</p>
				)
		}
```  

These are two very simple examples showing the simple differences between the two. One of the interesting thing is that a component's state can be passed down to another component as one of it's props. Like so:  

```
class iAmAComponent extends React.Component {
    state = {
		    count: 0
		}
		
		render() {
		    return(
				    <aCountingComponent count={this.state.count} />
				)
		}
``` 

This allows the *child* coponent access to the props (like properties, or like an argument) to be accessed as need be. State may only be accessed and changed by the component that it is within, but this allows that data to be distributed down through different components, making those components reusable as child components of different containers. Containers, you ask? That is for another post, but just think about a parent container that maniupulates it's state and passes that information down to other, more specific components (*child components*) as props. This allows each compnent to be coded for it's specific purpose (i.e. a button or some type if data display feature) and reused with different containers that might need to pass it different information to use.  

And that is a simple explanation of state and props.   




