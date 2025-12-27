# SimpleEQ 

This is an audio equalizer plugin built with JUCE and C++. 
It is a stereo 3-band equalizer consiting of: 
+ Low cut (high pass) filter
+ Peak filter
+ High cut filter

The project utilizes JUCE's dsp module, Processor Chain, IIR filters, and AudioProcessorValueTree state. 
I built this project to learn how EQ's work under the hood.

## Features

+ Stereo processing
+ Adjustable Parameters:
  + Low-cut frequency
  + Low-cut slope (12 / 24 / 36 / 48 dB per octave)
  + Peak frequency
  + Peak gain
  + Peak Q
  + High-cut frequency
  + High-cut slope
+ Response Curve display that shows the changes being heard

## Project Structure 
+SimpleEQ/
  + Source/
    + PluginProcessor.h
    + PluginProcessor.cpp
    + PluginEditor.h
    + PluginEditor.cpp
  + README.md
  + SimpleEQ.filtergraph
  + simpleEQ.jucer

## Requirements 
+ JUCE framework
+ C++17
+ Xcode(MacOS) or Visual Studio(Windows)
+ A DAW supporting VST3 or AU

## Building the plugin
1. Open SimpleEQ.jucer in Projucer
2. Export the project for your IDE
3. Build the plugin
4. Load it into your DAW

## What I learned
This project was built to practice and understand:
+ Audio EQ fundamentals
+ DSP filter design
+ Parameter handling with AudioProcessorValueTreeState
+ Real-time safe audio processing in C++

## What I am still working on 
+ Developing the GUI

## Aknowledgements 
I followed this tutorial along with reading the JUCE documentation: https://www.youtube.com/watch?v=i_Iq4_Kd7Rc&t=1798s
