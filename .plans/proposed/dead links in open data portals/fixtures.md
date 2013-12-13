days: 0.5


Make a server that does these things so I can use them as fixtures.

1. Serve a tiny file
2. Return a tiny file with error status codes
3. Serve a large file
4. Return a large file with error status codes

In the most awesome case, the thing I write can request just the
headers rather than downloading the whole dataset.

Actually, I guess I can use a HEAD request. But I wonder whether
everything supports that. I think it would be nicest if I could
do GET requests but only look at the first few lines.
