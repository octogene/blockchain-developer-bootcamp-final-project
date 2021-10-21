# Final Project

Final project for the Consensys Blockchain Developer Bootcamp 2021.

## Idea

Smart contract that allows any owner of a Twitter account to create an NFT
from any of his tweets and only his tweets.

## Workflow

1. User needs to open registration as the Twitter account owner :
```
function openRegistration(address _account, string _twitterHandle) returns (string) {
	// Open registration to link _twitterHandle to _account
	// Generate a string and returns it to the user
	// The string will need to be added to a tweet
}
```

2. User needs to confirm registration :

```
function confirmRegistration(address _account, uint tweetId) {
    // Check with oracle for the tweet and string
    // Confirm registration status of the user
}
```

3. User can mint any of its tweet :

```
function mintTweet(uint tweetId) {
    // Check with oracle that the tweet is owned by the user
    // Mint the tweet
}


