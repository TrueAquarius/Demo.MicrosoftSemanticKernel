﻿# Demo.MicrosoftSemanticKernel.LightPlugin

This project is a plugin for controlling lights, integrated with the Microsoft Semantic Kernel. It provides the following features:

- Retrieve the status of all lights
- Turn lights on and off
- Change the color of a light

## Features

### 1. `GetLightsAsync`
- **Description**: Retrieves a list of all lights and their current status.
- **Return Value**: A list of `LightModel`.

### 2. `TurnOnLightAsync`
- **Description**: Turns on a light based on its ID.
- **Parameters**: 
  - `id` (int): The ID of the light.
- **Return Value**: A message describing the new status of the light.

### 3. `TurnOffLightAsync`
- **Description**: Turns off a light based on its ID.
- **Parameters**: 
  - `id` (int): The ID of the light.
- **Return Value**: A message describing the new status of the light.

### 4. `SetLightColorAsync`
- **Description**: Changes the color of a light based on its ID.
- **Parameters**: 
  - `id` (int): The ID of the light.
  - `hex` (string): The new color value in HEX format.
- **Return Value**: A message describing the new status of the light.

## Prerequisites

- .NET 8 SDK
- Visual Studio 2022 or later
- C# 12.0
- Azure OpenAI Service 

## Configuration
- Set the following environment variables:
  - `AZURE_OPENAI_ENDPOINT`: The endpoint for the Azure OpenAI service.
  - `AZURE_OPENAI_API_KEY`: The API key for the Azure OpenAI service.
  - `AZURE_OPENAI_DEPLOYMENT_NAME`: The deployment name for the Azure OpenAI service.

## Notes

- At the time when this demo was created, the Semantic Kernel framework seemed to still undergo a lot of changes. Therefore these code examples may not work in future releases of that framework.
- Microsoft Semantic Kernel version 1.49.0 was used for this demo.

## Links

Here are a couple of links which 'inspired' this demo:
- [YouTube - Dev Leader - How To Use Semantic Kernel Plugins In C#](https://www.youtube.com/watch?v=1GjIY-F91jU)


## License

This project is licensed under the [MIT License](../LICENSE.txt).

   
   