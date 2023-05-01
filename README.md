# Automated parsing of Zoom meeting transcripts

This is an automatic parser of Zoom meeting transcripts that outputs MS Word documents (docx).

Compatible with Python 3+.

Just populate an input file, called `input.vtt`, where the output is the audio transcript from a Zoom call.

Once you've created your `input.vtt` file, you simply need to run the script with Python:
```
$ python process_zoom_transcript.py -s Speaker1 input.vtt processed_transcript.docx
Output file: processed_transcript.docx
```

The output file name will be printed on successful parsing. 

Multiple speaker names can be provided and only those lines will be retained. If multiple lines belong to the same speaker, they will be merged into a single paragraph in the output Word document.