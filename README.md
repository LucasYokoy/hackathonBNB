# HACKATHON BNB CPBR14

A solution for privacy, security and use empowerment for patients over their own medical data.

# OpenHealthChain

The blockchain provides an opportunity for the creation of a decentralized and private system for sharing healthcare information and still protect the client's privacy. That's where OpenHealthChain steps in, providing a new dimension to the open health concept.

Our goal is to use blockchain technology to allow patients to share their medical record with all doctors in a secure and private way. This is done creating an on chain "non-transferable NFT" claiming ownership of the patient's wallet over a PDF document containing medical information. These tokens will hereafter be refered to as Medical Record Tokens or MRTs.

An MRT contains a decentralized claim of ownership of the patient over a PDF file containing medical information. This ensures the client has true ownership of their MRTs, instead of the laboratory, doctor, or even OpenHealthChain itself. This also provides interoperability since the patient could transfer their medical files to the storage media of their choice and they would still be certifiable by the MRT.

# Content

On this repository, we have a ready to deploy smart contract written in Solidity. The code uses OpenZeppelin audited and certified contracts to ensure security and smooth functioning.
The contracts used were the ERC165 for eventual upgradeability. For the contract itself, we used a modified version of the ERC721 standard, where the transferFrom, safeTransferFrom, and safeTransfer functions were deleted. This is essentially what makes each MRT a "non-transferable NFT". 
We also made the ERC721 contract not Ownable, so anyone could mint their own MRTs.
