# non-equilibrium FDT in a Hopf whole-brain model

Here you can find the data and codes to apply the non-eq FDT formalism to wakefulness (W) and deep sleep (N3) data (see Monti _et al._ [https://www.biorxiv.org/content/10.1101/2024.04.04.588056v1](https://www.biorxiv.org/content/10.1101/2024.04.04.588056v1).

The code is written in MATLAB, and the files' names reflect the order in which the code should be executed (filenames start with the letter a because MATLAB does not allow filenames to begin with a number).


## The Data: 

In the _Data/Sleep_ directory you will find:

1. DataSleepW_N3.mat file: containing the structural connectivity (C), and the time-series (TS) for the W and N3 states for 15 subjects in each group (not necessarily the same subjects). The parcellation of each time-series corresponds to the AAL90.
2. Files hopf_freq_AAL90_COND_1_W.mat and hopf_freq_AAL90_COND_2_N3.mat containing the frequencies for each node (parcel) to be used in the whole-brain Hopf model. Throughout the code CONDITION 1 corresponds to W and CONDITION 2 to N3.
3. Compute_Hopf_Freq_AAL90_subs.m file: containing the code to obtain the nodes frequencies from the empirical TS for each condition.
4. gaussfilt.m: Gauss filter used in Compute_Hopf_Freq_AAL90_subs.m


## The Code:

1. a0_Ceff_fitting: this code fits the Effective Connectivity (EC) starting from the structural connectivity C (see Supplementary Material in Monti _et al._ [https://www.biorxiv.org/content/10.1101/2024.04.04.588056v1](https://www.biorxiv.org/content/10.1101/2024.04.04.588056v1).ç
2. 
