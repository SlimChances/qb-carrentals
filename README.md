# QBCore | CAR RENTALS | Time Based Car Renting System for QBUS Servers
CAR RENTAL system for QBUS Servers, Easy Functionality, and Highly Customizable. 


### [PREVIEW](https://youtu.be/pki6ms0_Ods)

## FEATURES 
[Lots of stuff! So please watch the Video!](https://youtu.be/swaYNDMAJmo)

## SETUP
- **Run the SQL file included with the REPOSITORY**
- Check the config.lua and make necessary changes. 
- Change fxversion in fxmanifest as required. 

## go to qb-inventory/html/js/app.js and near line 570 add this 
          } else if (itemData.name == "stickynote") {
                $(".item-info-title").html('<p>' + itemData.label + '</p>')
                $(".item-info-description").html('<p>' + itemData.info.label + '</p>');
            } else if (itemData.name == "rentalpapers") {
                $(".item-info-title").html('<p>' + itemData.label + '</p>')
                $(".item-info-description").html('<p><strong>Name: </strong><span>'+ itemData.info.firstname + '</span></p><p><strong>Last Name: </strong><span>'+ itemData.info.lastname+ '</span></p><p><strong>Plate: </strong><span>'+ itemData.info.plate + '<p><strong>Model: </strong></p>');

## Add this to qb-core/shared/items.lug
["rentalpapers"]				 = {["name"] = "rentalpapers", 					["label"] = "Rental Papers", 			["weight"] = 0, 		["type"] = "item", 		["image"] = "rental.png", 		["unique"] = true, 		["useable"] = false, 	["shouldClose"] = false, 	["combinable"] = nil, 	["description"] = "Yea, this is my car i can prove it!"},
## CREDITS
- SlimChancesGaming_FB#1602 For The re-write (NOT ORIGINAL DEV!)
- Alen and Ariz for Patiently Testing the Script for me! These guys are awesome!
- MonkeyWhisper and ixTooT for Suggesting Improvements to the original devs. 




