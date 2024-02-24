# Angular Charts Integration using ng2 Charts

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 15.0.0.

## Installation

    Install ng2-charts using npm

npm install --save ng2-charts

    Install Chart.js library

npm install --save chart.js

## Usage

In order to use ng2-charts you need to import NgChartsModule:

import { NgChartsModule } from 'ng2-charts';

// In your App's module:
imports: [
  NgChartsModule
]

## Global configuration

When you import NgChartsModule you can pass a global configuration object to it:

import { NgChartsModule } from 'ng2-charts';

// In your App's module:
imports: [
  NgChartsModule.forRoot({ defaults: { ... } })
]

Alternatively, include a provider in your module, or one of the parent modules:

import { NgChartsModule, NgChartsConfiguration } from 'ng2-charts';

imports: [
  NgChartsModule
],
providers: [
  { provide: NgChartsConfiguration, useValue: { generateColors: false }}
]

## Additional configuration

Install libraries if required, for example -

<!-- For adding datalables plugins -->
npm install chartjs-plugin-datalabels 