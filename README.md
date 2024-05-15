# A Quantum of QUIC: Dissecting Cryptography with Post-Quantum Insights

This repository containes additional data for the paper *A Quantum of QUIC: Dissecting Cryptography with Post-Quantum Insights*, by Marcel Kempf, Nikolas Gauder, Benedikt Jaeger, Johannes Zirngibl, and Georg Carle.
The paper was published at [IFIP Networking 2024](https://networking.ifip.org/2024/).

If you could find our work useful, consider citing our paper. 
You can use:

```bibtex
@inproceedings{kempf2024quiccrypto,
  title = {{A Quantum of QUIC: Dissecting Cryptography with Post-Quantum Insights}},
  author = {Kempf, Marcel and Gauder, Nikolas and Jaeger, Benedikt and Zirngibl, Johannes and Carle, Georg},
  booktitle = {International Federation for Information Processing (IFIP) Networking Conference 2024},
  address = {Thessaloniki, Greece},
  year = 2024,
  month = jun,
  keywords = {quic, performance measurements, post-quantum cryptography},
}
```


## Modified TLS Libraries

The modified TLS libraries used for measurements are published in the following repositories:

* [OpenSSL](https://github.com/tumi8/openssl-quic-noop)
* [BoringSSL](https://github.com/tumi8/boringssl-noop)

We also provide Git patches for both libraries in the [noop-patches](/noop-patches) folder. You can use them to try to quickly apply the needed changes for a no-op cipher on current versions of the TLS libraries.

## Other Resources

We use the modified QUIC Interop Runner from the "QUIC on the Highway: Evaluating Performance on High Rate Links" paper. The framework and scripts for postprocessing and analysis are available [here](https://github.com/tumi8/quic-10g-paper).