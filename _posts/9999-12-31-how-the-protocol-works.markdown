The RTB Connect uses a custom XML-based protocol.  
The example lines I show will show `>>` for lines of data sent from the server and `<<` for lines of data sent from the client.  
When the connection is opened the server always sends this to the client (of course without the `>>` in the beginning):

    >> <notice type="welcome"><version>1.0</version></notice>

This line will not be included in the other example conversations.
