# Breaking RSA Encryption

## Introduction
The project aims at decrypting the RSA algorithm via brute forcing and use of few intelligent algorithms. This program tries to calculate prime numbers p & q using distributed computing which determines phi and then decrypts the encrypted number by brute-force way.
In September 2000, the US patent for the RSA algorithm expired, for the first time enabling software developers everywhere to freely include this PKC standard in their products.
Refer the wiki for more details http://en.wikipedia.org/wiki/RSA_(cryptosystem)

## Usage
### Server
This has to be run on all the nodes, including the primary node.

	$ rmiregistry
	$ java Server

### Primary
The program distributes the numbers to be computed uniformly amongst the number of available nodes.

	$ java Main [ip1] [ip2] [...]
	
## Example
Main.java has the variables defined as the following.

	BigInteger n=new BigInteger("721498723487");
	BigInteger e=new BigInteger("71");
	BigInteger encryptedNumber=new BigInteger("2790");

Other set working integers are as follows.
	
	{53390003, 235} = {17715907, 53390003}
	{37600133, 743} = {31364807, 37600133}
	{2868729161, 587} = {2800199471, 2868729161}
	{239072460563, 1187} = {15307017707, 239072460563}
	{25775503209341, 2095} = {5917905368239, 25775503209341}
	{49818871, 81} = {28899049, 49818871}
	{496303695959, 181} = {408558235285, 496303695959}
	{19638286331501, 121} = {1298398434217, 19638286331501}
	{566530045212367, 521} = {182681457184889, 566530045212367}

## License

MIT: http://vineetdhanawat.mit-license.org/
