# Fetch the metadata of NFT

* NFT metadata is stored in cloud storage like AWS S3 or a distributed storage like IPFS.
* It is written by the JSON format and each NFT owners can define their own key and value.
* Because, NFT standard ERC-721 do not support the metadata storage (it has only metadata URL), programmer has to fetch each metadata through that URL.
* In order to solve this problem, many services provides way to fetch all metadata for each NFT collection.
* Here, we will show two kinds of sample code. One is for direct fetch way using metadata URL, but this is very slow and not easy way. The other one is way using Alchemy API, and this is very effective to fetch NFT metadata for programmer.
* You can test a sample code for a direct fetching way.
  * [https://codesandbox.io/s/fetch-nft-metadata-from-token-url-9vm976?file=/src/App.js:646-725](https://codesandbox.io/s/fetch-nft-metadata-from-token-url-9vm976?file=/src/App.js:646-725)
* You can test a sample code for a Alchemy fetching way.
  * [https://codesandbox.io/s/fetch-the-nft-metadata-with-alchemy-api-2k7mzt?file=/src/App.js](https://codesandbox.io/s/fetch-the-nft-metadata-with-alchemy-api-2k7mzt?file=/src/App.js)
