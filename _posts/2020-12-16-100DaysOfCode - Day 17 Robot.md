---
title: 100DaysOfCode - Day 17 Robot
categories:
- 100DaysOfCode
- CSS_flexbox
feature_image: "https://picsum.photos/2560/600?image=872"
layout: post
---

This project is easy and fun!

> This is my project: [Day17_robot](https://portfolio.tsainei.com/100DaysOfCode/Day17_robot/) and my [code](https://github.com/tsainei/portfolio/tree/main/100DaysOfCode/Day17_robot)

My CSS:

```
h1 {
	text-align: center;
	font-family: 'Roboto', sans-serif;
}

.robots {
	flex-wrap: wrap;
	display: flex;
	justify-content: center;
}

.head, 
.left_arm, 
.torso, 
.right_arm, 
.left_leg, 
.right_leg {
	 background-color: #7d5fe8;
}

.head { 
	width: 200px; 
	margin: 0 auto; 
	height: 150px; 
	border-radius: 200px 200px 0 0; 
	margin-bottom: 10px;
} 

.eyes {
	display: flex;
}

.head:hover {
	width: 300px;
    transition: 1s ease-in-out;
}

.upper_body { 
	width: 300px; 
	height: 150px;
	display: flex; 
} 

.left_arm, .right_arm { 
	width: 40px; 
	height: 125px;
	border-radius: 100px; 
} 

.left_arm { 
	margin-right: 10px; 
	transition: all 3s;
} 

.left_arm:hover {
	transform: translate(10px, 20px);
}

.right_arm { 
	margin-left: 10px; 
	transition: all 1s;
} 

.right_arm:hover {
	transform: rotate(-90deg);
}

.torso { 
	width: 200px; 
	height: 200px;
	border-radius: 0 0 50px 50px; 
	transition: all 3s 1s;
} 

.torso:hover {
  transform: skew(25deg, 10deg);
}

.lower_body { 
	width: 200px; 
	height: 200px;
	/* This is another useful property. Hmm what do you think it does?*/
	margin: 0 auto;
	display: flex;
} 

.left_leg, .right_leg { 
	width: 40px; 
	height: 120px;
	border-radius: 0 0 100px 100px; 
} 

.left_leg { 
	margin-left: 45px; 
} 

.left_leg:hover {
	  -webkit-transform: rotate(20deg);
    -moz-transform: rotate(20deg);
    -o-transform: rotate(20deg);
    -ms-transform: rotate(20deg);
    transform: rotate(20deg);
}

.right_leg { 
	margin-left: 30px; 
  transition: all 1s;
}

.right_leg:hover {
	transform: rotate(-40deg);
}

.left_eye, .right_eye { 
	width: 20px; 
	height: 20px; 
	border-radius: 15px; 
	background-color: white; 
} 

.left_eye { 
	position: relative; 
	top: 100px; 
	left: 40px; 
	transition: all 1s; 
} 

.left_eye:hover {
	transform: translate(20px, 20px);
}

.right_eye { 
	position: relative; 
	top: 100px; 
	left: 120px; 
	transition: all 2s;
}

.right_eye:hover {
	transform-origin: left top;
	transform: rotate(720deg);
}
```