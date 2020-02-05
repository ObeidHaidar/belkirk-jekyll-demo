---
heading: Belkirk College
sub_heading: Engineering and Health Sciences
layout: home
title: test
banner_image: ''
hero_button:
  text: ''
  href: ''
textline: ''
services: []
show_news: false
partners: []
show_staff: false
published: false

---
## Q4
Assume L = 4

```matlab
Steered_wheel_angles=[-5 10 -40 35 -15 0];
v=2;L=4;
figure
for i=1:length(Steered_wheel_angles)
    subplot(2,3,i);
    x=0;y=0;theta_0=0;
    theta_dot=tand(Steered_wheel_angles(i))*v/L + theta_0;
    for t=0:0.1:2
        x(end+1)=x(end)+v*cos(theta_dot*t);
        y(end+1)=y(end)+v*sin(theta_dot*t);
    end
    plot(x,y,'-')
    axis([-5 40 -15 15]);
    grid on
    title(["Steering Angle",Steered_wheel_angles(i)])
end
```
![](md_media/C4Q4.png)