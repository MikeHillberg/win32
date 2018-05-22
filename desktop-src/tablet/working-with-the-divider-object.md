---
Description: 'The Divider object provides access to the Tablet PC layout analysis features.'
ms.assetid: '9fa299fe-3713-4fa8-95c6-be15f144103a'
title: Working with the Divider Object
---

# Working with the Divider Object

The [Divider](frlrfMicrosoftInkDividerClassTopic) object provides access to the Tablet PC layout analysis features.

In managed code, the [Divider](frlrfMicrosoftInkDividerClassTopic) object can be instantiated by calling one of the [Divider](frlrfMicrosoftInkDividerClassctorTopic) constructors. In Automation, this is called the [**InkDivider**](inkdivider-class.md) object, and it can be instantiated by calling the [**CoCreateInstance**](com.cocreateinstance) method in C++.

You can obtain a snapshot of the current analysis result by calling the [Divide](frlrfMicrosoftInkDividerClassDivideTopic) method of the [Divider](frlrfMicrosoftInkDividerClassTopic) object. The analysis result is returned in a [DivisionResult](frlrfMicrosoftInkDivisionResultClassTopic) object. Each time you call the Divide method, the Divider object creates a DivisionResult object. For more information about the DivisionResult object, see [Working with the DivisionResult Object](working-with-the-divisionresult-object.md).

The [Strokes](frlrfMicrosoftInkStrokesClassTopic) collection that the [Divider](frlrfMicrosoftInkDividerClassTopic) object analyzes is contained in the [Strokes](frlrfMicrosoftInkDividerClassStrokesTopic) property of the Divider object. The Divider object dynamically analyzes the Strokes collection as you add to or delete from the collection. For more information about the Strokes property of the Divider object, see [Working with a Strokes Collection](working-with-a-strokes-collection.md).

The [Divider](frlrfMicrosoftInkDividerClassTopic) object uses a recognizer context to improve its analysis of recognition segments and to generate recognition text for handwriting elements. You can set the recognizer context by using the [RecognizerContext](frlrfMicrosoftInkDividerClassRecognizerContextTopic) property of the Divider object. The RecognizerContext property cannot be changed after strokes have been assigned to the Divider object. For more information about the RecognizerContext property of the Divider object, see [Working with a Recognizer Context](working-with-a-recognizer-context.md).

> \[!Caution\]  
> In managed code, you must call the [Dispose](frlrfMicrosoftInkDividerClassDisposeTopic) method on this object before it goes out of scope. This object maintains non-managed resources. Relying on finalization for this object can cause memory leaks and exceptions within your application.

 

 

 


