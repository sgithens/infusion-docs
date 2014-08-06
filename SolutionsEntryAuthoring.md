# Writing GPII Solutions Registry Entries

This document will show step by step how to write a new solutions registry entry
for the GPII. In this tutorial we will write an entry for Jaws, a widely used
screen reader for Microsoft Windows. Jaws is proprietary software, but a trial 
development version can be installed for our purposes. For this tutorial we will
not be attempting to cover all the features of JAWS, we will be creating just
a basic solutions entry that covers one or two preferences.

This tutorial is version controlled, and may change as the GPII codebase evolves.
For example, some steps in this tutorial are temporary requirements that will
change or go away as the GPII feature set evolves. Steps in the tutorial that may
go away in future versions of the GPII will be noted as they are presented when
possible.

## Prerequisites

You should have a working GPII development environement setup, and be familier
with starting and stopping the system, as well as logging in as certain personas.
Instructions for setting up the GPII development environment can be found here TODO.

The example solution application here is JAWS. A demo version can be downloaded and 
installed from here. TODO. Once you have installed JAWS, do the following to set up
a JAWS profile to use. This is a work around for this basic tutorial.  

In JAWS, a profile should be created by going to "options"->voices->Voice Adjustment. 
Make sure that "Eloquence - (factory)" is selected in the profile name. 
Click "Save As.." button and write "cloud4all" as the name (no quotes). Once this is 
done, Jaws should be working properly

## Overview of steps.

Writing a solutions registry entry consists largely of writing configuration in 
JSON format that is plugged in to the GPII at various places. For this tutorial 
we will also be using javascript to write tests cases.

Our work flow will be:

* Adding hooks and registrations for our entry to GPII configuration. This involves
  adding our entry id to things like the device reporter, and create test personas
  that use our new solution.
* Writing the full solutions JSON that contains all the information for starting,
  stopping, and configuring JAWS, as well as the capabilities it provides, and any
  environment dependencies it might have.
* Writing acceptance tests that test our solution. For long term development this is 
  vital to automating the test and release process for the GPII.

## Tutorial Steps

### Step 1: Pick a solution ID

### Step 2: Add your solution to the device reporter payload

### Step 3: Create demo persona to test with

### Step 4: Add the solutions entry to the registry JSON

### Add the solutions contexts

### Add the settings handlers

### Add the lifecycle actions
