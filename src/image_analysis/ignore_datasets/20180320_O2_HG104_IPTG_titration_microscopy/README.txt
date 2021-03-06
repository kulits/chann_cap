#Date : 2018-03-20
#Equipment : Artemis Nikon microscope
#User : mrazomej
#Description : 
#IPTG titration of the O2 - HG104 strain.
#Strains :
#> HG105 galK::25 / pZS3-mCherry (auto)
#> HG105 galK::25-O2+11-YFP / pZS4-mCherry (delta)
#> HG104 galK::25-O2+11-YFP / pZS4-mCherry
#
#The strains were grown overnight in tubes in 3 mL of LB + spec + kan. 
#Next morning they were diluted 1:1000 into 0.5 mL of M9 + 0.5% glucose 
#also in deep 96-well plates.
#The auto and delta strains were grown without IPTG
#The analysis strain was grown with the following IPTG concentrations
#IPTG concentrations:
#0uM, 0.1uM, 5uM, 10uM, 25uM, 50uM, 75uM, 100uM, 250uM, 500uM, 1000uM, 5000uM
#After 8 hours the cells were diluted 1:10 into M9 + glucose and imaged
#using 2% agar pads also of M9 media.
#
#Microscope settings:
#100x Oil objective
#Exposure time:
#> Brightfield : 2 ms
#> mCherry : 13 ms
#> YFP : 550 ms
#
#Comments :
# It was particularly difficult to find lots of positions for concentration
# 75 µM so there are less pictures for this concentration.
# VERY IMPORTANT: The microscope was set to TIRF illumination, on the mCherry
# channel. What this means is that the segmentation might not have been the 
# best since it reduces the area by ≈ 30%.
