---
layout: post
title:  "Masters thesis"
date:   2015-07-26 15:05:08
categories: [thesis, cognitive science, affective computing]
summary: "My masters thesis on improving the game of Tetris through physiological signals such as heart rate, skin conductance and facial muscles."
---
This is the thesis I worked on from September 2013 to February 2014.

The title is **Improving game experience using dynamic difficulty adjustment based on physiological signals**

##Summary

The goal of this thesis is to investigate whether dynamic difficulty adjustment (DDA) based on emotions is better than DDA based on a player''s performance. DDA is a technique in computer games to change the difficulty of the game so that it meets a certain criteria. For the "emotion-based" DDA the goal is to keep the player in a state of Flow which was coined by Csikzentmihalyi. For the "performance-based" DDA the goal is to keep the player performing well without dying.

To accomplish this two DDA systems have to be built. Tetris was chosen as the game for the two DDA systems as difficulty could easily be controlled in Tetris.

The "emotion-based" DDA system uses physiological signals to recognize emotions. Based on the literature study the physiological signals chosen are heart rate (HR), temperature and galvanic skin response (GSR). Due to equipment availability HR (based on blood volume pulse(BVP)), GSR and electromyography (EMG) of the facial muscles were used instead. These signals were measured while 5 test participants played Tetris and "self-rated" their valence and arousal which could be translated into emotions later. Another test was made where test participants had to look at images and "self-rate" their valence and arousal. This test, or validation study, was made to ensure that the Tetris results were correct. Using the data from these tests a classifier was trained using a total of 44 features. The results were not good as they ranged from 22% to 46% with a chance level of 33%. Therefore the "emotion-based" DDA was changed to only using heart rate as it correlated with arousal. The new DDA tried to keep the player''s heart rate slightly elevated above the resting heart rate.

The "performance-based" DDA uses the game state to judge whether a change in difficulty is needed. The goal of the "performance-based" DDA is to keep the block height in Tetris in a certain level. If the block height is below the level then difficulty is increased and vice versa.

9 participants played both DDA versions and "self-rated" their arousal, valence and sense of challenge. The results of this experiment showed no statistically difference between the two DDA versions although a manual inspection of the results indicated that some participants might have preferred the "performance-based" DDA.

You can read the entire thing by downloading my thesis here:
[Download]({{site.assets_folder}}thesis.pdf)
