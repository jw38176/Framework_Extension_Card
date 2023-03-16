# Journal 

## Inspiration 

The goal of this project is to design a USB-C extension card for the framework laptop: an all modular thin-and-light laptop. It puts traditionally hard to repair laptops to shame and fostered a very welcoming open source community. Although the Framework story didn't make it into my report on the lifespan of corporate backed open source communities since it is still too young, I would like to dedicate the non-written component to participating in the extension card deisgn sub-community. 

### Motivation and Aim

When I set out to make an extension card, I was both happy and sad to find an extension card CAD design for almost anything - SD cards, WiFi cards, dual USB, magnetic charging, and even a storage space at the side of the laptop, or a side scroll wheel that is already in production?? I was amazed at the creativity of the makers, and it was a delight to find out that most of the projects they post are also open source, and if you want to buy one they only charge 3D printing cost and shipping. However, I was left scratching my head thinking about what I should do. 

Then I remembered an issue that has been plaguing my laptop for a long time - electronic interference on the 3.5mm headphone jack. Whenever I use my in-ear headphones with my laptop, there is a constant whining noise and occasional beeping. After some investigating, I concluded that it wasn't a driver issue or a sample rate issue, but rather small electrical leaks in the system that was interfering with the audio line. Will this affect the safety or operation of my laptop in any way? No. Is it annoying? Yes. 

So I set my sights on making a headphone jack extension card. There are 2 differences that this will have compared to the built-in headphone jack. For one, the audio signal will be coming from the USB port, which are generally less prone to interference. The other is that the extension card would have a built-in DAC, which not only enables the USB signal to 3.5 audio conversion but also somewhat increases the quality of sound (highly dependent on what DAC is used). 

To ensure that the project is accessible to everyone, the electronics will be modelled after available products on Amazon instead of the typical approach of printing custom PCBs. The models will also have 3D printing in mind, and have relatively simple designs. 

## Mark 1 

The first prototype was modelled after this type of adapter: 

<img src="/img/adapter1.png"  width="400" height="400">
<img src="/img/adapter1ad.png"  width="400" height="400">

Unfortunately, they did not have any CAD models available, but there was a rough dimensions specification. After getting the dimensions of the extension card and looking at available designs on the forum, this is my first design: 

<img src="/img/mark1a.png"  width="600" height="400">
<img src="/img/mark1b.png"  width="600" height="400">
<img src="/img/mark1c.png"  width="600" height="400">
<img src="/img/mark1d.png"  width="600" height="400">
<img src="/img/mark1e.png"  width="600" height="400">

The bottom half that holds the adapter is slightly indented into the bottom board to accomodate the relatively large adapter. The user would insert the adapter in from above, and insert the extension card into the laptop. 

This design has loads of problems. For one, because the extension card is so small in height, the adapter would actually be touching the top of the laptop frame when plugged in, potentially scratching the laptop. This also makes it impossible to make a lid for the extension card, and in turn make the card very infeasible to swap around with other extension cards (since you have to insert the adapter into the extension card and insert the extension card into the laptop, why not just use the adapter :> ). Another flaw is that this adapter is not very popular, and most people would need to go out and buy the adapter for the extension card to work. 

In conclusion, there is a lot of room for improvement, but I gained a lot of experience both in CAD and designing this specific extension card. 

## Mark 2

For the second generation, I have decided to use this as the adapter instead: 

<img src="/img/adapter2.png"  width="400" height="400">

This has its own drawbacks, the worst being that since the extension card is so small, it can not accommodate the entire adapter leaving a coil sticking out. However, since most people have one of these lying around and it is considerably thinner than the last adapter, I think this would be the best option for now. 

To make the prototype more realistic, I found a model of a generic USB-C to 3.5mm audio jack adapter and used it as the reference. 

This is the Mark 2 CAD design: 

<img src="/img/bottom1.png"  width="600" height="400">
<img src="/img/bottom2.png"  width="600" height="400">
<img src="/img/lid1.png"  width="600" height="400">
<img src="/img/lid2.png"  width="600" height="400">
<img src="/img/mark2c.png"  width="600" height="400">
<img src="/img/mark2d.png"  width="600" height="400">
<img src="/img/mark2e.png"  width="600" height="400">
<img src="/img/mark2f.png"  width="600" height="400">
<img src="/img/mark2g.png"  width="600" height="400">


Both the extrusion on the lid and hole for the wire to come out are slightly smaller than they should be, to accommodate errors and inaccuracies in 3D printing. The lid is secured by 2 screws modelled after a 3mm flathead screw. There are also cavities in the extension card to save filament when 3D printing. 

The most notable improvement is that it now has a lid which secures the adapter in place. This makes the prototype truly a functional extension card. Another advantage of this design is that it fits a large range of adapters of the same type. Just simply change the dimension of 2 blocks and it will fit on your own adapter! 

## Current State

Mark 2 is the latest iteration that I have, and I plan to take this further with 3D printing prototypes and more testing. If there are any suggestions on or issues you have with the current design feel free to leave a message in the repository!
