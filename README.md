# Houston Railroad Crossing Blockage Prediction Agent 🚂 🛤️
### ITAI 2376 — Deep Learning in Artificial Intelligence | Houston City College

![Python](https://img.shields.io/badge/Python-3.12-blue)
![LangChain](https://img.shields.io/badge/LangChain-0.2.16-green)
![PyTorch](https://img.shields.io/badge/PyTorch-2.3.0-orange)
![GPT](https://img.shields.io/badge/LLM-GPT--3.5--Turbo-purple)
![Accuracy](https://img.shields.io/badge/GRU%20Accuracy-85.0%25-brightgreen)
---

This project uses historical data from the Federal Railroad Administration (FRA) and a GRU deep learning model to predict the probability that a railroad crossing in Houston, Texas will be blocked by a train, proactively alerting emergency dispatchers and city planners based on predicted risk level.

## The Problem
This project was inspired by living in the Houston, Texas neighborhood of Eastwood for nearly a decade. The neighborhood is defined by a high concentration of railroad crossings, where stopped trains regularly impede traffic for minutes to hours at a time. Beyond the inconvenience to drivers, the blocked crossings pose a significant public safety risk forcing first responders to seek detours and wasting critical response time in the process.

Since 2021, Texas has led the nation in blocked crossings according to publicly available data from the [FRA](https://www.fra.dot.gov/blockedcrossings/incidents). In the first half of 2025, the Houston Fire Department was blocked 643 times with half of those calls resulting in delays ([KHOU, 2025](https://www.khou.com/article/news/local/houston-rail-crossings-blocked-by-stopped-trains/285-f59f3d0c-ef28-48fe-8658-790ee95fb748)). Eastwood Street alone recorded 2,277 blockage reports between 2020 and 2026 with an increasing trend year over year.

Despite initiatives in recent years, including the City of Houston's [Smart Railroad Crossings](https://www.houstontx.gov/council/committees/tti/20220512/Smart-Railroad-Crossing-Monitors-Pilot.pdf) pilot program, a study by [TRAINFO](https://trainfo.ca/wp-content/uploads/47415-TR-Trainfo-White-Paper-FINAL-Web.pdf), and the launch of [Train Watch](https://houstontx.gov/trainwatch/) in 2025, no publicly available tool proactively predicts when a crossing will be blocked and recommends a course of action before emergency vehicles are impacted. This agent seeks to fill that void using only publicly available FRA data, making it accessible without the need for proprietary hardware or paid APIs. It was built with the community of Houston in mind, to serve as a tool for emergency dispatchers to make informed decisions based on proactive alerts and for city planners who need pattern analysis data to justify infrastructure investment decisions.

## Option Chosen

![Architecture Diagram](architecture.png)
