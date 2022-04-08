# Overview
WhiteSource matches your source files to the source library (from GitHub, SourceForge, or other SCM) from which they most likely originated, done by utilizing a set of advanced algorithms. WhiteSource’s knowledge base includes ~340M source files and ~45M open-source projects (source libraries). 

# SmartMatch
WhiteSource’s newest source files matching algorithm (called SmartMatch) is powered by a machine learning engine and takes approximately 5x more parameters into consideration when determining your source files' original repository than the previous Weight algorithm. In addition to that, as more and more of our customers adopt our source file matching capabilities, we gain experience and improve in fine-tuning the algorithm's weight allocation of different parameters. 

# Coverage
One of the major challenges we encounter when trying to match source files to their original source library is creating a potential matching pool encompassing the major hosts which distribute the source libraries. Over the past year, we have significantly expanded our reach in regards to the hosts we cover, adding numerous additional hosts to our list.

# Removing Third Party Tags/Files
Another challenge is automatically determining which source files constitute part of the source library, and which constitute third-party components that the source library is dependent on. We've implemented detection for file paths that hint at a probable third-party component, and source files found within these folders are filtered out during the matching algorithm. 

# Testing with WhiteSource
This repository contains an example of the scan open source component using the [Unified Agent](https://whitesource.atlassian.net/wiki/spaces/WD/pages/804814917/Unified+Agent+Overview)
[SourceFileMatching.yml](https://github.com/Dima2021/SourceFileMatching-Demo/blob/main/.github/workflows/SourceFileMatching.yml)
