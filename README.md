# Besties-GPT

This app enables AI-powered search for the ALL IN podcast.

App is here:
https://besties-gpt.fly.dev 

## Dataset
 
Use whisper to generate transcripts with all steps outlined in -
`scripts/make_index.ipynb`
 
 ## App

Use Langchain `VectorDBQAChain` to - 
* Embed the user query
* Perform similarity search on Pinecone embeddings
* Synthesize the answer from relevant chunks with `GPT 3.5` (also benchmark GPT4)

Relevant chunks with metadata (links) are displayed as source documents.
 
This builds on the excellent UI from https://github.com/mckaywrigley/wait-but-why-gpt.

## Deploy

Deploy to Fly.io: `fly launch`

## Credits

Thanks to [Mckay Wrigley](https://twitter.com/mckaywrigley) for open-sourcing his UI.
 
Thanks to All IN for the excellent podcast.

## Local testing

`yarn dev`

## Contact

If you have any questions, feel free to reach out to me on [Twitter](https://twitter.com/RLanceMartin)!
