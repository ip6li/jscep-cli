# Build

```bash
$ https://github.com/ip6li/jscep-cli.git
$ cd jscep-cli
$ mvn compile
$ mvn package
$ java -jar target/jscepcli-1.2-jar-with-dependencies.jar
```

# Usage

```bash
Usage: <main class> [options]
  Options:
    --algorithm
      BouncyCastle signature algorithm to use
      Default: SHA256
    --ca-certificate-file
      CACert output file
      Default: cacert.pem
    --ca-identifier
      CA identifier (try AdminCA1 if using a default EJBCA install)
    --certificate-file
      Certificate output file
      Default: cert.pem
    --challenge
      Challenge password (EJBCA entity password)
    --crl-file
      CRL output file
      Default: crl.pem
    --csr-file
      CSR output file
    --dn
      Subject DN to request
    --existingCsrFile
      Pre created CSR file (PEM format), requires --existingKeyFile
    --existingKeyFile
      Pre created key file (PEM format), requires --existingCsrFile
    --key-file
      Private key output file
      Default: privkey.pem
    --keySize
      Size of key, if you want more than 2048, you need the JCE
      Default: 2048
    -t, --text
      Output PEM-format objects on stdout. (similar to 'openssl <cmd> -text')
      Default: false
  * --url
      SCEP URL. For EJBCA, use 
      http://<hostname>:<port>/ejbca/publicweb/apply/scep/pkiclient.exe 
    -v, --verbose
      Verbose output
      Default: false
```
