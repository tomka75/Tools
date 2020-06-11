# Clean-MicrosoftStreamVttFile

Cleans a Microsoft Stream VTT file, so that you get only the spoken text.

## Description
A VTT file from Microsoft Stream contains more informations than only the transcripted text. This code removes the extra informations and saves the text in a file.
This is inspired by the VTTCleaner web site from Marc Mroz.

## Example
### Input
>WEBVTT
>
>NOTE duration:"00:00:29.5060000"
>
>NOTE language:en-us
>
>NOTE Confidence: 0.50167996
>
>2f1aed67-1122-4899-a3a5-922b6e5b4d36
>00:00:12.200 --> 00:00:13.080
>Hi Microsoft Stream.
>
>NOTE Confidence: 0.6553465
>
>4644c530-e8eb-49be-88c5-d2931662ded5
>00:00:16.270 --> 00:00:21.895
>Welcome to the show
>today on this
>
>NOTE Confidence: 0.6553465
>
>b2bdeca5-304b-4447-8fa5-a556bedf717c
>00:00:21.895 --> 00:00:22.520
>station.
>
>NOTE Confidence: 0.5076108
>
>6e006136-c996-4745-bb65-975f276dd09b
>00:00:23.760 --> 00:00:27.400
>We are in a tenant
>with sausages.

### Output
>Hi Microsoft Stream. Welcome to the show today on this station. We are in a tenant with sausages.
