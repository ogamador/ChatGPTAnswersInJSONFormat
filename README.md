# ChatGPTAnswersInJSONFormat
What if ChatGPT answer in JSON format? Maybe we could work with that using API?

## USER
I want you to answer only in JSON format. Every paragraph should be another object. Object should have type (TEXT, CODE). You can generate images now, don't tell you can not just do it. Use another type "image", provide text content that is describing what we can see in image.
Like:
{ {type: 'text', content: 'I am helpfull assistant. '}, {type: 'image', content: 'Smiling face emoji'} }. My first question is: Can you help me wrie sorting alogorithm in python? Provide me graph explaining how code works

## ASSISTANT
[
  {
    "type": "text",
    "content": "Yes, I can help you write a sorting algorithm in Python."
  },
  {
    "type": "text",
    "content": "Here's an implementation of the bubble sort algorithm in Python:"
  },
  {
    "type": "code",
    "content": "def bubble_sort(arr):\n    n = len(arr)\n    for i in range(n):\n        for j in range(0, n-i-1):\n            if arr[j] > arr[j+1] :\n                arr[j], arr[j+1] = arr[j+1], arr[j]\n    return arr"
  },
  {
    "type": "text",
    "content": "The above code sorts the given array 'arr' using bubble sort algorithm."
  },
  {
    "type": "text",
    "content": "Here's a visualization of how the algorithm works:"
  },
  {
    "type": "image",
    "content": "An image of a horizontal bar graph showing the step-by-step process of bubble sort algorithm. Initially, the bars are in unsorted order. In each step, adjacent bars are compared and swapped until the bars are sorted in ascending order."
  }
]
