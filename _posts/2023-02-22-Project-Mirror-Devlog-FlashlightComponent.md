---
layout: post
title:  "How To Make A Flashlight Component in UE5 using C++"
date:   2022-03-28 08:22:38 +0200
categories: UE5 C++ Components Flashlight
regenerate: true
---

# How To Make A Flashlight Component in C++

Flashlights are very easy to create in C++ as they are essentially Spotlight Components that are already built into the Engine

![](/assets/Images/ActivateFlashlight.png)

First create a new C++ class in the editor and select a Spotlight Component as the base class


Then in the header file add in 2 new variables:

```c++

public:
  UPROPERTY(BlueprintReadOnly, EditDefaultsOnly)
  float Flashlight = 100;
  
  UPROPERTY(BlueprintReadOnly)
  bool bIsEnabled = false;
  
 ```
