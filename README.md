# bread_analysis
Code to characterize the performance of the Harvard BREAD DAQ. All dependencies for the enviornment are basic numpy etc. and listed at the top of the main cell for each notebook.

adu_waterfall.ipynb shows characterizing the RFI occuring during these averaging tests and in the surrounding environment of the receiver chain.

hopping_averaging_prototyping.ipynb shows testing several different hopping methods including the final selection of Gaussian, along with development of a statistical framework for characterizing how aligned the results are with the radiometer equation's scaling that is used in SNR_scaling_pipeline.ipynb. Included is also an attempt to do a hot/cold test with a fixed ENR noise source injection averaging run compared against a terminated end averaging run.

SNR_v_time.ipynb works with a long averaging run and shows the resulting SNR v. time aligns with the scaling prediction of the radiometer equation.

timing_masking_check.ipynb shows timing the data acquistion and offloading process and attempting to dynamically mask RFI.
