# Local storage

**Cookies downsides:**

- Cookies will be sent everytime we make an http request which will put stress on traffic.

- Cookies may be sniffed by hackers if the application were not encrypted via SSL.

- Cookies are limited by it's size (4 kb).

**What we need in our web apps is huge space on client side that will persist under page refresh and it's not sent over internet.**

**Storage event object:**

- it has a key.
- an old value.
- a new value.
- and a url that will hold the page that we call it from.

```javascript

function saveGameState() {
    if (!supportsLocalStorage()) { return false; }
    localStorage["halma.game.in.progress"] = gGameInProgress;
    for (var i = 0; i < kNumPieces; i++) {
	localStorage["halma.piece." + i + ".row"] = gPieces[i].row;
	localStorage["halma.piece." + i + ".column"] = gPieces[i].column;
    }
    localStorage["halma.selectedpiece"] = gSelectedPieceIndex;
    localStorage["halma.selectedpiecehasmoved"] = gSelectedPieceHasMoved;
    localStorage["halma.movecount"] = gMoveCount;
    return true;
}




```


**all interested implementors have used an equivalent SQL backend (Sqlite), but we'd like multiple independent implementations to proceed along a standardisation path. Until another implementor is curious about implementing this spec, the outline of the SQL dialect has been left as simply a regard to Sqlite, which isn't suitable for a standard.**

