# How does the model learn RAG?

<video src="${PRIVATE_VIDEO_RAG_1}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

LLMs learn much like humans do—by seeing examples, understanding patterns, and applying that knowledge. In Retrieval-Augmented Generation (RAG), we train the model by showing it examples known as ‘data samples’ that combine retrieving relevant information with generating accurate responses. This helps the model learn how to fetch useful data and provide better answers.

These data samples play a crucial role in the RAG training process. It involves 4 basic steps as shown below.

<img height="300" width="900" src="${PRIVATE_IMAGE_RAG_1}" />

Let’s understand this and create a data sample with a working example in the upcoming section.