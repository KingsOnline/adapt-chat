# adapt-chat

**Chat** is a *presentation component* Created by the King's Online Dev team.

<img src="https://cdn.rawgit.com/KingsOnline/repo-files/f54de408/chat.gif" alt="An example of the Chat component">

The **Chat** component offers scenario based learning. It recreates a "group chat" that two or more people may have on a messaging platform.

## Settings Overview

The attributes listed below are used in *components.json* to configure **Chat**, and are properly formatted as JSON in *example.json* file. In the Authoring Tool use the attributes below.

### Attributes

For core model attributes see [**core model attributes**](https://github.com/adaptlearning/adapt_framework/wiki/Core-model-attributes). The attributes listed below are specific to the `Chat` component.

**_button** (object): This allows you to specify the default button text (Optional).

>**continueText** (string): The text to display to trigger the next item (Optional - defaults to "Next")

**_participants** (object): This allows you to specify the participants in the chat (Optional).

>**name** (string): The name of the participant

>**_icon** (string): An image of the participant


**_items** (array): Each item represents a line of text of the chat.

>**body** (string): The text for the line of the chat.

>**_participant** (number): The participant who said this line, from the *_participants* object. Note that the first participant is 0, the second is 1 etc.

>**_timeToShow** (number): The number of seconds to show this line. If the *_button* is enabled the time to show the button. Otherwise the time for the line to be invoked.

>**_button** (object): Lines can be invoked by a button or automatically

 >**_button._isEnabled** (boolean): Decide if this line should have a button that invokes it.

>**_button.buttonText** (text): The text of the button for this line.

## Limitations

No known limitations

----------------------------
**Version number:**  2.0.0
**Framework versions:** >= 2.0
**Author / maintainer:** [Simon Date](mailto:simon.date@kcl.ac.uk)
