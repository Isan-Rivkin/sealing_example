# Project Title

Pure Enclave in rust and App (untrusted in C).


### Prerequisites


* [RUST-SGX-SDK](https://github.com/baidu/rust-sgx-sdk/blob/master/documents/sgxtime.md) - follow the instalation rules
* clone this repo into /some/path/sealing_example
* run docker 
``` 
 docker run -v baidu/sdk/repo/path/rust-sgx-sdk/:/root/sgx -v /some/path/sealing_example:/root/sealing_example -v -ti --device /dev/isgx baiduxlab/sgx-rust
```
* Inside docker: 
```
 /opt/intel/sgxpsw/aesm/aesm_service &
 ```

```
cd /root/sealing_example
```

```
make
```

```
cd bin/
```

* Run the binary 

```
./app
```