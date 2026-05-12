# GE_QED
Files for the Price-Hancock Debate of 2026 - in which Genetic Entropy is demonstrated.

The main SLiM code file I used for the simulation I showed in the debate came from:

human_scaled_3_v3.slim

IMPORTANT NOTE:

I now realize that the density-dependent fitness scaling of my simulation was acting to artificially slow down the process of genetic entropy. The following alteration to the code should work to mitigate this for future runs:

early() {
    if (p1.individualCount > K)
        p1.fitnessScaling = K / p1.individualCount;
    else
        p1.fitnessScaling = 1.0;
}

URLs for public Google Sheets data and Flourish visualization:

https://docs.google.com/spreadsheets/d/1N_l3YEErHo8Hoe2zFgr0gCe14Sl3b3HgbMJhU33Emgk/edit?usp=sharing

https://docs.google.com/spreadsheets/d/1hoFRlW8tHRxKN658og-dOiav2ysj_9Np4gc5PpxLpWc/edit?usp=sharing

https://public.flourish.studio/story/3639943/
