Flow-on-Auto_Encoder-Latent



Modular Circuit Diagram:

[Input Image] --> [Spectrum Dataset] --> [Amplitude & Phase Spectra]
                     |                     |                  |
                     v                     v                  v
               [Data Loader]         [Encoder1]          [Encoder2]
                     |                     |                  |
                     |------------------> [Concatenate] <----|
                                          |       |
                                          v       v
                                    [Normalizing Flow]
                                          |
                                          v
                                      [Decoder]
                                          |
                                          v
                                 [Reconstructed Image]
