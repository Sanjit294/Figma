# Ex09 Event Registration Web Application
## Date: 17/05/25

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:

```
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { Input } from "@/components/ui/input";
import React from "react";

export default function IphoneSe(): JSX.Element {
  const formFields = [
    { id: "fullName", label: "Full Name" },
    { id: "gender", label: "Gender" },
    { id: "age", label: "Age" },
    { id: "email", label: "Email ID" },
    { id: "registerNo", label: "Register no" },
    { id: "department", label: "Department" },
    { id: "event", label: "Event to Register" },
  ];

  return (
    <div className="bg-white flex flex-row justify-center w-full">
      <div className="bg-white w-80 h-[568px]">
        <div className="relative h-[568px] bg-[url(/background-1.png)] bg-cover bg-[50%_50%]">
          {/* Header / College Logo */}
          <header className="absolute w-80 h-[49px] top-0 left-0">
            <img
              className="w-full h-full object-cover"
              alt="Saveetha Engineering College Logo"
              src=""
            />
          </header>

          {/* Event Title */}
          <div className="absolute w-[220px] h-[25px] mt-[71px] left-1/2 transform -translate-x-1/2">
            {[1, 2, 3].map((index) => (
              <h1
                key={index}
                className="absolute w-[220px] [font-family:'PoetsenOne-Regular',Helvetica] font-normal text-white text-xl tracking-[0] leading-[28.0px] whitespace-nowrap"
              >
                Sports Day Events
              </h1>
            ))}
          </div>

          {/* Registration Form Card */}
          <Card className="absolute w-[251px] h-[357px] top-[110px] left-[38px] rounded-[26px] bg-[#d9d9d9] border border-solid border-[#000000b0] opacity-45">
            <CardContent className="p-0 pt-[10px]">
              {formFields.map((field) => (
                <div key={field.id} className="relative mt-[26px]">
                  <Input
                    id={field.id}
                    placeholder={field.label}
                    className="absolute w-[209px] h-[22px] left-[19px] bg-[#d9d9d9] rounded-[var(--shape-corner-extra-large)] text-black text-[13px] pl-[15px]"
                    style={{ fontFamily: "Lekton-Regular, Helvetica" }}
                  />
                </div>
              ))}
            </CardContent>
          </Card>

          {/* Register Button */}
          <Button className="absolute h-[26px] top-[494px] left-[118px] bg-transparent hover:bg-transparent p-0">
            <div className="relative w-[84px] h-[26px]">
              <img
                className="absolute w-[81px] h-[26px] top-0 left-0"
                alt="Register button background"
                src=""
              />
              <span
                className="absolute w-16 top-[3px] left-5 font-normal text-black text-xs tracking-[0] leading-[16.8px] whitespace-nowrap"
                style={{ fontFamily: "Leckerli_One-Regular, Helvetica" }}
              >
                Register
              </span>
            </div>
          </Button>

          {/* Thank You Message */}
          <section className="absolute w-[246px] h-[53px] top-[155px] left-7">
            <h1 className="absolute w-[204px] top-[9px] left-9 [font-family:'Lemon-Regular',Helvetica] font-normal text-black text-[32px] tracking-[-0.32px] leading-[44.8px] whitespace-nowrap">
              Thank You
            </h1>
          </section>

          {/* Contact Card */}
          <Card className="absolute w-[303px] h-[137px] top-[259px] left-2 bg-[#d9d9d9] rounded-[20px] opacity-45 border-none">
            <CardContent className="p-0">
              <h2 className="absolute w-[220px] top-[11px] left-[92px] [font-family:'PoetsenOne-Regular',Helvetica] font-normal text-white text-xl tracking-[0] leading-[28.0px] whitespace-nowrap">
                Contact Us
              </h2>
              <p className="absolute w-[244px] top-[55px] left-9 [font-family:'Leckerli_One-Regular',Helvetica] font-normal text-[#0a0808] text-[13px] tracking-[0] leading-[18.2px]">
                saveethaengineeringcollege@gmail.com
              </p>
              <p className="absolute w-[188px] top-[97px] left-[100px] [font-family:'Leckerli_One-Regular',Helvetica] font-normal text-[#531313] text-[13px] tracking-[0] leading-[18.2px] whitespace-nowrap">
                7395454900
              </p>
            </CardContent>
          </Card>
        </div>
      </div>
    </div>
  );
}
```

## OUTPUT:

![alt text](<Screenshot 2025-05-17 150526.png>)
![alt text](<Screenshot 2025-05-17 150604.png>)
![alt text](<Screenshot 2025-05-17 150613.png>)
![alt text](<Screenshot 2025-05-17 150623.png>)
![alt text](<Screenshot 2025-05-17 150631.png>)


## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
