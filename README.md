#  HWS Project 9

In this project, we are adding to projcet 7 to use GCD and prevent hangups when lading a URL using webkit. 

We used _DispatchQueue.global_ to move the loading of JSON to a background thread. This caused some UI issues, so we then moved _parse_ and _showError_ methods from the background to the main thread using _DispatchQueue.main_

Next, we re-factored the code using the _performSelector(inBackground:)_  to make the calls to background theads a little cleaner looking.
