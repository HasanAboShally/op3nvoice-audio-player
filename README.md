OP3Nvoice Audio Player
======================

This is a proof of concept audio player that integrates with the OP3Nvoice search library.

This uses the PHP library available here: https://github.com/Op3nvoice/op3nvoice-php

To use this:
*  you should only have to configure your API Key (line 8) and set the audio duration (line 57). This audio duration will be available from the search results eventually.
*  download the OP3Nvoice PHP library from above and simply copy the src/ and vendor/ directories into the root directory of the player.
*  then add your search terms via the url. It should look something like this:

http://localhost/op3nvoice-player/?terms=something

http://localhost/op3nvoice-player/?terms=close|monkey|desert|does



This can be improved in a number of ways:

*  this only shows the first resulting file, we could extend it to show all of them;
*  the duration should be included in the API call so we don't have to hardcode it here (line 57);
*  if there are no search results, we could display a more useful/friendly message.
