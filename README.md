# UNIX-Assignment
This is yawei's unix assignment. In this assignment, there are two data files for me to inspect and analysis. My UNIX assignment consists two components: The inspection of data The processing of these same data files to produce output files that are formatted for a subsequent analysis. The workflow and the codes for both data inspection and processing are as following:
### Data inspection
```
$ mkdir Data-inspection
```

```
$wc fang_et_al_genotypes.txt
```

The number of lines, words, and bytes (characters) in  fang_et_al_genotypes.txt are 2783  2744038 11051939 

```
wc snp_position.txt
```
The number of lines, words, and bytes (characters) in snp_position.txt are 984 13198 82763 

```
$ head -1 fang_et_al_genotypes.txt
```
Sample_ID	JG_OTU	Group	abph1.20	abph1.22	ae1.3	ae1.4	ae1.5	an1.4	ba1.6	ba1.9	bt2.5	bt2.7	bt2.8	Fea2.1	Fea2.5	id1.3	lg2.11	lg2.2	pbf1.1	pbf1.2	pbf1.3	pbf1.5	pbf1.6	pbf1.7	pbf1.8	PZA00003.11	PZA00004.2	PZA00005.8	PZA00005.9	PZA00006.13	PZA00006.14	PZA00008.1	PZA00010.5	PZA00013.10	PZA00013.11	PZA00013.9	PZA00015.4	PZA00017.1	PZA00018.5	PZA00029.11	PZA00029.12	PZA00030.11	PZA00031.5	PZA00041.3	PZA00042.2	PZA00042.5	PZA00043.7	PZA00045.1	PZA00047.2	PZA00049.12	PZA00050.9	PZA00051.2	PZA00058.5	PZA00058.6	PZA00060.2	PZA00061.1	PZA00065.2	PZA00069.4	PZA00070.5	PZA00078.2	PZA00079.1	PZA00081.17	PZA00084.2	PZA00084.3	PZA00086.8	PZA00088.3	PZA00090.2	PZA00092.1	PZA00092.5	PZA00093.2	PZA00096.26	PZA00097.13	PZA00098.14	PZA00100.10	PZA00100.12	PZA00100.14	PZA00100.9	PZA00103.20	PZA00106.9	PZA00107.18	PZA00108.12	PZA00108.14	PZA00108.15	PZA00109.3	PZA00109.5	PZA00111.2	PZA00111.4	PZA00111.5	PZA00111.6	PZA00111.8	PZA00114.3	PZA00116.2	PZA00119.4	PZA00120.4	PZA00123.1	PZA00125.2	PZA00131.14	PZA00132.17	PZA00132.18	PZA00132.3	PZA00135.6	PZA00137.2	PZA00139.14	PZA00140.10	PZA00140.6	PZA00140.9	PZA00142.6	PZA00148.2	PZA00153.3	PZA00153.6	PZA00163.4	PZA00164.1	PZA00164.2	PZA00164.3	PZA00166.1	PZA00166.3	PZA00170.1	PZA00170.3	PZA00170.4	PZA00174.1	PZA00174.2	PZA00175.2	PZA00176.8	PZA00177.4	PZA00178.3	PZA00182.3	PZA00182.4	PZA00184.1	PZA00184.4	PZA00188.1	PZA00188.3	PZA00191.5	PZA00192.6	PZA00192.7	PZA00193.2	PZA00198.39	PZA00200.11	PZA00200.17	PZA00200.9	PZA00201.2	PZA00204.1	PZA00210.1	PZA00210.6	PZA00211.7	PZA00212.1	PZA00213.19	PZA00214.1	PZA00216.9	PZA00218.1	PZA00218.6	PZA00219.7	PZA00220.11	PZA00220.12	PZA00221.7	PZA00225.8	PZA00226.7	PZA00227.8	PZA00230.5	PZA00232.24	PZA00234.21	PZA00235.6	PZA00235.8	PZA00237.2	PZA00237.7	PZA00237.8	PZA00238.3	PZA00240.9	PZA00241.6	PZA00243.27	PZA00245.14	PZA00245.16	PZA00245.17	PZA00245.18	PZA00245.19	PZA00249.2	PZA00250.1	PZA00251.1	PZA00254.3	PZA00255.15	PZA00255.17	PZA00256.16	PZA00256.21	PZA00256.23	PZA00257.11	PZA00257.22	PZA00261.6	PZA00263.14	PZA00266.5	PZA00270.3	PZA00273.1	PZA00274.7	PZA00277.17	PZA00277.9	PZA00280.14	PZA00287.1	PZA00289.11	PZA00294.20	PZA00296.6	PZA00297.2	PZA00297.3	PZA00297.4	PZA00298.4	PZA00298.5	PZA00299.2	PZA00300.12	PZA00300.13	PZA00300.14	PZA00300.16	PZA00301.3	PZA00303.19	PZA00303.21	PZA00307.12	PZA00307.14	PZA00307.17	PZA00309.2	PZA00310.5	PZA00314.6	PZA00314.8	PZA00315.1	PZA00315.6	PZA00318.2	PZA00323.3	PZA00323.4	PZA00326.16	PZA00326.18	PZA00326.19	PZA00332.8	PZA00332.9	PZA00334.2	PZA00335.12	PZA00337.3	PZA00337.4	PZA00337.5	PZA00342.9	PZA00344.10	PZA00345.15	PZA00346.1	PZA00346.2	PZA00346.3	PZA00349.3	PZA00349.5	PZA00350.2	PZA00352.22	PZA00355.1	PZA00355.2	PZA00356.9	PZA00364.5	PZA00364.6	PZA00367.2	PZA00369.1	PZA00370.1	PZA00370.5	PZA00380.5	PZA00380.7	PZA00381.3	PZA00381.4	PZA00381.5	PZA00382.17	PZA00385.3	PZA00386.3	PZA00390.6	PZA00391.2	PZA00392.3	PZA00392.4	PZA00393.1	PZA00393.4	PZA00394.11	PZA00395.1	PZA00395.2	PZA00396.12	PZA00401.11	PZA00401.6	PZA00406.1	PZA00407.9	PZA00408.7	PZA00409.3	PZA00411.1	PZA00411.4	PZA00411.5	PZA00413.17	PZA00413.18	PZA00413.21	PZA00417.2	PZA00417.3	PZA00419.1	PZA00420.4	PZA00422.2	PZA00422.5	PZA00422.6	PZA00423.16	PZA00423.17	PZA00424.1	PZA00425.4	PZA00425.9	PZA00429.1	PZA00433.5	PZA00436.7	PZA00439.6	PZA00440.1	PZA00442.3	PZA00442.4	PZA00442.5	PZA00442.6	PZA00444.1	PZA00444.5	PZA00445.18	PZA00449.2	PZA00452.4	PZA00458.6	PZA00459.5	PZA00460.3	PZA00460.5	PZA00460.7	PZA00462.2	PZA00463.3	PZA00466.1	PZA00468.11	PZA00468.7	PZA00470.1	PZA00471.2	PZA00471.3	PZA00471.4	PZA00472.2	PZA00477.10	PZA00477.11	PZA00477.5	PZA00477.9	PZA00478.10	PZA00478.11	PZA00478.7	PZA00478.9	PZA00480.10	PZA00481.7	PZA00484.5	PZA00485.2	PZA00486.2	PZA00487.16	PZA00487.24	PZA00487.26	PZA00489.1	PZA00493.1	PZA00493.2	PZA00493.5	PZA00495.3	PZA00495.4	PZA00495.6	PZA00496.1	PZA00497.1	PZA00497.4	PZA00498.4	PZA00499.10	PZA00499.12	PZA00499.3	PZA00501.12	PZA00501.14	PZA00502.5	PZA00503.5	PZA00504.1	PZA00504.2	PZA00505.4	PZA00505.8	PZA00510.2	PZA00510.3	PZA00514.1	PZA00514.6	PZA00514.7	PZA00515.14	PZA00516.3	PZA00517.6	PZA00522.12	PZA00523.2	PZA00525.16	PZA00525.2	PZA00527.6	PZA00527.9	PZA00529.3	PZA00531.1	PZA00533.3	PZA00533.4	PZA00533.5	PZA00533.6	PZA00534.2	PZA00536.2	PZA00538.12	PZA00538.16	PZA00538.8	PZA00543.2	PZA00543.4	PZA00543.5	PZA00545.21	PZA00545.22	PZA00545.4	PZA00547.13	PZA00547.18	PZA00552.4	PZA00560.1	PZA00560.2	PZA00562.4	PZA00565.3	PZA00566.5	PZA00568.19	PZA00573.3	PZA00578.1	PZA00579.6	PZA00582.4	PZA00586.1	PZA00587.3	PZA00587.6	PZA00588.2	PZA00588.4	PZA00589.10	PZA00589.8	PZA00589.9	PZA00593.2	PZA00595.3	PZA00600.11	PZA00603.1	PZA00608.1	PZA00608.5	PZA00610.18	PZA00610.9	PZA00613.22	PZA00614.12	PZA00615.3	PZA00615.6	PZA00615.8	PZA00617.16	PZA00618.22	PZA00620.2	PZA00621.2	PZA00622.1	PZA00622.2	PZA00623.2	PZA00626.3	PZA00626.4	PZA00630.9	PZA00636.5	PZA00636.6	PZA00637.4	PZA00639.12	PZA00639.13	PZA00639.15	PZA00641.7	PZA00641.8	PZA00644.11	PZA00647.9	PZA00650.8	PZA00654.10	PZA00654.12	PZA00655.1	PZA00656.15	PZA00656.16	PZA00656.18	PZA00656.4	PZA00658.19	PZA00658.23	PZA00662.3	PZA00665.6	PZA00667.1	PZA00672.6	PZA00672.8	PZA00673.2	PZA00674.3	PZA00676.2	PZA00680.1	PZA00680.3	PZA00682.2	PZA00684.12	PZA00686.8	PZA00692.5	PZA00693.3	PZA00695.1	PZA00698.4	PZA00700.3	PZA00704.11	PZA00705.5	PZA00706.16	PZA00710.1	PZA00710.16	PZA00712.4	PZA00715.3	PZA00717.14	PZA00719.1	PZA00719.2	PZA00719.3	PZA00720.2	PZA00720.3	PZA00721.4	PZA00721.5	PZA00725.4	PZA00726.6	PZA00726.7	PZA00726.9	PZA00727.11	PZA00727.12	PZA00729.18	PZA00729.19	PZA00730.2	PZA00731.6	PZA00731.7	PZA01104.1	PZA01149.1	PZA01149.3	PZA01182.1	PZA01240.1	PZA01240.2	PZA01420.1	PZA01420.2	PZA01420.3	PZA01474.2	PZA01637.2	PZA01637.3	PZA01637.4	PZA01725.1	PZA01725.2	PZA01782.2	PZA01782.3	PZA01782.4	PZA02789.31	PZA02789.36	PZA02791.6	PZA02792.16	PZA02792.9	PZA02806.4	PZA02806.9	PZA02807.5	PZA02808.12	PZA02808.16	PZA02819.35	PZA02820.6	PZA02822.2	PZA02824.1	PZA02824.3	PZA02825.8	PZA02831.5	PZA02837.5	PZA02844.1	PZA02850.18	PZA02850.4	PZA02853.10	PZA02853.7	PZA02856.1	PZA02862.3	PZA02865.11	PZA02869.2	PZA02869.8	PZA02872.1	PZA02872.3	PZA02878.12	PZA02888.3	PZA02890.3	PZA02890.4	PZA02890.5	PZA02894.1	PZA02897.12	PZA02906.12	PZA02906.7	PZA02921.9	PZA02923.7	PZA02927.1	PZA02938.5	PZA02939.6	PZA02940.3	PZA02941.3	PZA02941.6	PZA02941.8	PZA02947.2	PZA02948.19	PZA02948.21	PZA02948.22	PZA02949.22	PZA02949.26	PZA02952.10	PZA02954.2	PZA02955.3	PZA02958.17	PZA02959.7	PZA02961.1	PZA02962.13	PZA02963.5	PZA02966.11	PZA02968.4	PZA02969.11	PZA02970.9	PZA02972.1	PZA02982.5	PZA02982.6	PZA02983.38	PZA02984.7	PZA02988.2	PZA02993.5	PZA02997.16	PZA02997.19	PZA03001.15	PZA03001.18	PZA03001.9	PZA03009.5	PZA03009.6	PZA03009.7	PZA03009.8	PZA03011.6	PZA03012.10	PZA03013.7	PZA03013.8	PZA03014.10	PZA03014.21	PZA03014.24	PZA03017.10	PZA03017.11	PZA03024.16	PZA03024.18	PZA03024.7	PZA03028.5	PZA03032.16	PZA03034.1	PZA03035.5	PZA03037.8	PZA03037.9	PZA03041.8	PZA03042.1	PZA03042.5	PZA03046.2	PZA03046.3	PZA03047.12	PZA03047.20	PZA03047.22	PZA03048.16	PZA03048.17	PZA03049.23	PZA03051.1	PZA03051.3	PZA03052.15	PZA03054.3	PZA03054.5	PZA03058.17	PZA03062.15	PZA03062.7	PZA03063.17	PZA03063.18	PZA03064.6	PZA03067.17	PZA03067.20	PZA03068.11	PZA03068.13	PZA03069.6	PZA03073.23	PZA03073.24	PZA03074.24	PZA03078.33	PZA03081.1	PZA03081.10	PZA03081.11	PZA03081.13	PZA03081.6	PZA03083.7	PZA03089.12	PZA03090.31	PZA03092.7	PZA03094.18	PZA03094.6	PZA03095.1	PZA03095.2	PZA03095.3	PZA03097.4	PZA03097.7	PZA03097.9	PZA03102.10	PZA03102.2	PZA03102.9	PZA03137.1	PZA03172.2	PZA03223.3	PZA03258.2	PZA03283.2	PZA03284.3	PZA03290.1	PZA03290.2	PZA03295.4	PZA03296.6	PZA03296.7	PZA03298.1	PZA03298.2	PZA03301.2	PZA03301.4	PZA03302.1	PZA03305.6	PZA03305.7	PZA03311.2	PZA03311.3	PZA03311.4	PZA03311.5	PZA03312.1	PZA03312.2	PZA03316.2	PZA03317.1	PZA03319.3	PZA03319.4	PZA03320.3	PZA03320.4	PZA03328.5	PZA03329.1	PZA03329.2	PZA03333.3	PZA03335.2	PZA03335.3	PZA03337.1	PZA03338.5	PZA03340.2	PZA03342.2	PZA03344.4	PZA03344.5	PZA03344.6	PZA03345.1	PZA03345.2	PZA03345.4	PZA03347.1	PZA03348.1	PZA03349.1	PZA03349.9	PZA03767.1	PZA03767.4	PZA03767.5	PZA03773.2	PZA03773.3	PZA03774.1	PZA03774.10	PZA03774.2	PZA03774.4	PZA03774.5	PZA03774.6	PZA03774.8	PZA03774.9	PZA03775.1	PZA03775.11	PZA03775.2	PZA03775.3	PZA03775.4	PZA03775.6	PZA03775.7	PZA03775.8	PZA03775.9	PZA03781.1	PZA03781.2	PZA03781.3	PZA03781.4	PZA03781.5	PZA03781.6	PZA03781.7	PZA03781.8	PZA03782.1	PZA03782.3	PZA03786.1	PZA03786.2	PZA03789.1	PZA03789.2	PZA03789.4	PZB00011.4	PZB00011.5	PZB00041.2	PZB00041.4	PZB00049.2	PZB00049.4	PZB00049.7	PZB00055.1	PZB00060.4	PZB00062.6	PZB00062.7	PZB00062.8	PZB00067.2	PZB00067.3	PZB00067.4	PZB00067.5	PZB00078.1	PZB00081.2	PZB00081.4	PZB00081.5	PZB00081.7	PZB00092.1	PZB00092.4	PZB00093.3	PZB00093.4	PZB00093.6	PZB00096.2	PZB00096.3	PZB00136.3	PZB00140.1	PZB00145.2	PZB00149.2	PZB00149.4	PZB00153.1	PZB00153.2	PZB00153.3	PZB00153.5	PZB00160.1	PZB00160.2	PZB00160.4	PZB00165.2	PZB00165.6	PZB00169.4	PZB00169.6	PZB00175.1	PZB00175.2	PZB00175.3	PZB00175.4	PZB00175.5	PZB00180.1	PZB00180.2	PZB00183.3	PZB00188.6	PZB00207.3	PZB00221.3	PZB00221.8	PZB00229.3	PZB00232.1	PZB00232.2	PZB00232.4	PZB00232.5	PZB00379.3	PZB00379.4	PZB00379.5	PZB00393.7	PZB00409.3	PZB00416.2	PZB00416.5	PZB00454.2	PZB00454.3	PZB00454.4	PZB00454.5	PZB00498.2	PZB00498.4	PZB00598.1	PZB00598.2	PZB00603.3	PZB00603.4	PZB00603.5	PZB00607.2	PZB00761.1	PZB00761.2	PZB00849.2	PZB00849.3	PZB00849.4	PZB00859.1	PZB01109.2	PZB01109.3	PZB01110.1	PZB01110.2	PZB01110.3	PZB01111.6	PZB01111.7	PZB01111.8	PZB01112.3	PZB01112.4	PZB01112.5	PZB01112.6	PZB01113.4	PZB01114.1	PZB01114.3	PZB01115.1	PZB01115.5	PZB01115.6	PZB01116.2	PZB01221.1	PZB01222.1	PZB01222.3	PZB01223.3	PZB01223.4	PZB01223.7	PZB01225.1	PZB01225.2	PZB01225.4	PZB01228.1	PZB01228.3	PZB01228.4	PZB01233.2	PZB01233.3	PZB01238.5	PZB01238.6	PZB01427.1	PZB01427.3	PZB01463.2	PZB01463.3	PZB01463.4	PZD00003.1	PZD00003.3	PZD00007.1	PZD00008.3	PZD00011.1	PZD00011.3	PZD00011.4	PZD00012.1	PZD00012.2	PZD00012.3	PZD00012.4	PZD00012.5	PZD00013.3	PZD00013.4	PZD00014.3	PZD00017.1	PZD00019.1	PZD00020.2	PZD00020.3	PZD00020.4	PZD00020.6	PZD00021.2	PZD00021.4	PZD00021.5	PZD00022.1	PZD00022.3	PZD00022.4	PZD00024.2	PZD00025.1	PZD00025.2	PZD00030.1	PZD00030.4	PZD00030.5	PZD00030.6	PZD00034.3	PZD00043.1	PZD00043.2	PZD00043.3	PZD00043.4	PZD00044.2	PZD00044.3	PZD00044.4	PZD00045.1	PZD00045.2	PZD00045.3	PZD00045.4	PZD00049.3	PZD00049.4	PZD00049.5	PZD00051.1	PZD00052.3	PZD00052.4	PZD00062.2	PZD00066.1	PZD00067.1	PZD00067.2	PZD00067.3	PZD00068.1	PZD00069.2	PZD00069.3	PZD00069.4	PZD00069.5	PZD00073.1	PZD00073.2	PZD00073.6	PZD00074.1	PZD00075.1	PZD00075.2	PZD00076.1	PZD00076.2	PZD00076.4	PZD00077.10	PZD00077.5	PZD00077.7	PZD00077.8	PZD00078.2	Ra2_ORF.1	Ra2_ORF.2	Ra2_ORF.4	Ra2_promoter.1	Ra2_promoter.2	Ra2_promoter.3	sh2.5	sh2.6	sh2.7	sh2.9	su1.4	su1.5	su1.7	tb1.17	tb1.18	tb1.19	tb1.5	te1.3	te1.4	zagl1.1	zagl1.6	zap1.2	zen1.1	zen1.2	zen1.4	zfl2.6	zmm3.4

```
head -1 snp_position.txt
```
SNP_ID	cdv_marker_id	Chromosome	Position	alt_pos	mult_positions	amplicon	cdv_map_feature.name	gene	candidate/random	Genaissance_daa_id	Sequenom_daa_id	count_amplicons	count_cmf	count_gene

```
$ ls -lh fang_et_al_genotypes.txt
```
-rw-r--r--. 1 yaweil domain users 11M Sep 13 13:38 fang_et_al_genotypes.txt
file size 

```
ls -lh snp_position.txt
```
-rw-r--r--. 1 yaweil domain users 81K Sep 13 13:38 snp_position.txt
file size 

```
awk -F "\t" '{print NF; exit}' fang_et_al_genotypes.txt
```

the number of columns in fang_et_al_genotypes.txt are 986

```
awk -F "\t" '{print NF; exit}' snp_position.txt
```

the number of columns in snp_position.txt 15




## Data processing
when I do the data inspecting, I found that the first three column of fang_et_al_genotypes.txt cannot be uesd, so I want to delete them. when I cheched the remaining column of fang_et_al_genotypes.txt, I found the remaining columns can match the rows in snp_position.txt. o before I join them, I have to transposed the fang_et_al_genotypes.txt and delete all the headers in the files of fang_et_al_genotypes.txt and snp_position.txt. But I transpose the data after extracting the teosinte and maize data.

```
$ mkdir Data-Processing
```

```
$ egrep "ZMMLR|ZMMIL|ZMMMR|Sample_ID" fang_et_al_genotypes.txt > maize_fang_et_al_genotypes.txt 
```
###grep ZMMLR or ZMMIL or ZMMMR

```
$ egrep "ZMPBA|ZMPIL|ZMPJA|Sample_ID" fang_et_al_genotypes.txt > teosinte_fang_et_al_genotypes.txt 
```
###grep ZMPBA, ZMPIL, and ZMPJA

```
$ awk -f transpose.awk teosinte_fang_et_al_genotypes.txt > teosinte_transposed_genotypes.txt
```
###transpose the teosinte_fang_et_al_genotypes.txt

```
$ awk -f transpose.awk maize_fang_et_al_genotypes.txt > maize_transposed_genotypes.txt
```
###transpose the maize_fang_et_al_genotypes.txt

```
$ sed -i '1,3d' maize_transposed_genotypes.txt teosinte_transposed_genotypes.txt 
```
###delete Sample_ID, JG_OTU, and Group lines

```
$ sed '1d' snp_position.txt >snp_position_nohead.txt
```
###delete head of snp
```
$ sort -k1,1V snp_position_nohead.txt > snp_position_nohead_sorted.txt
```
```
$ sort -k1,1V maize_transposed_genotypes.txt > maize_transposed_genotypes_sorted.txt
```
###sort maize

```
$ sort -k1,1V teosinte_transposed_genotypes.txt > teosinte_transposed_genotypes_sorted.txt 
```
###sort teosinte

```
$ join -1 1 -2 1 -t $'\t' snp_position_nohead_sorted.txt maize_transposed_genotypes_sorted.txt > maize_transposed_genotypes_joined.bed
```
join snp with maize

```
$ join -1 1 -2 1 -t $'\t' snp_position_nohead_sorted.txt teosinte_transposed_genotypes_sorted.txt > teosinte_transposed_genotypes_joined.bed 
```
###join snp with teosinte

```
$ sort -k3,3 teosinte_transposed_genotypes_joined.bed > teosinte_transposed_genotypes_joined_chr.bed
```

sort chrom colum

```
$ grep -v "^#" teosinte_transposed_genotypes_joined_chr.bed | cut -f3 | uniq -c 
```

###count the amount of samples for each different chromosomes for group teosinte

---output---
    155 1
     53 10
    127 2
    107 3
     91 4
    122 5
     76 6
     97 7
     62 8
     60 9
      6 multiple
     27 unknown

```
$ sed -n '1,155p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr1.bed 
```

```
$ sed -n '156,208p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr10.bed
```
```
$ sed -n '209,335p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr2.bed
```
```
$ sed -n '336,442p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr3.bed
```
```
$ sed -n '443,533p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr4.bed
```
```
$ sed -n '534,655p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr5.bed
```
```
$ sed -n '656,731p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr6.bed
```
```
$ sed -n '732,828p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr7.bed
```
```
$ sed -n '829,890p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr8.bed
```
```
$ sed -n '891,950p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr9.bed
```
```
$ sed -n '951,956p' teosinte_transposed_genotypes_joined_chr.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_transposed_genotypes_joined_mutiple.bed
```
```
$ sed -n '957,983p' teosinte_transposed_genotypes_joined_chr.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_transposed_genotypes_joined_unknown.bed
```
```
$ sort -k4,4V teosinte_transposed_genotypes_joined_chr9.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr9_ordered_increased.bed 
```
ordered based on increasing position values and with missing data encoded by this symbol: ?

```
$ sort -k4,4V teosinte_transposed_genotypes_joined_chr8.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr8_ordered_increased.bed
```
```
$ sort -k4,4V teosinte_transposed_genotypes_joined_chr7.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr7_ordered_increased.bed
```
```
$ sort -k4,4V teosinte_transposed_genotypes_joined_chr6.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr6_ordered_increased.bed
```
```
$ sort -k4,4V teosinte_transposed_genotypes_joined_chr5.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr5_ordered_increased.bed
```
```
$ sort -k4,4V teosinte_transposed_genotypes_joined_chr4.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr4_ordered_increased.bed
```
```
$ sort -k4,4V teosinte_transposed_genotypes_joined_chr3.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr3_ordered_increased.bed
```
```
$ sort -k4,4V teosinte_transposed_genotypes_joined_chr2.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr2_ordered_increased.bed
```
```
$ sort -k4,4V teosinte_transposed_genotypes_joined_chr1.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr1_ordered_increased.bed
```
```
$ sort -k4,4V teosinte_transposed_genotypes_joined_chr10.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr10_ordered_increased.bed
```

decreasing position values and with missing data encoded by this symbol: -

```
$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr8.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr8_ordered_decreased.bed
```
```
$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr1.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr1_ordered_decreased.bed
```
```
$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr2.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr2_ordered_decreased.bed
```
```
$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr3.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr3_ordered_decreased.bed
```
```
$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr4.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr4_ordered_decreased.bed
```
```
$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr5.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr5_ordered_decreased.bed
```
```
$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr6.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr6_ordered_decreased.bed
```
```
$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr7.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr7_ordered_decreased.bed
```
```
$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr9.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr9_ordered_decreased.bed
```
```
$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr10.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr10_ordered_decreased.bed
```
```
$ sort -k3,3 maize_transposed_genotypes_joined.bed > maize_transposed_genotypes_joined_chr.bed 
```
###sort chrom colum

```
$ sed -n '1,155p' maize_transposed_genotypes_joined_chr.bed > maize_transposed_genotypes_joined_chr1.bed 
```
```
$ sed -n '156,208p' maize_transposed_genotypes_joined_chr.bed > maize_transposed_genotypes_joined_chr10.bed
```
```
$ sed -n '209,335p' maize_transposed_genotypes_joined_chr.bed > maize_transposed_genotypes_joined_chr2.bed
```
```
$ sed -n '336,442p' maize_transposed_genotypes_joined_chr.bed > maize_transposed_genotypes_joined_chr3.bed
```
```
$ sed -n '443,533p' maize_transposed_genotypes_joined_chr.bed > maize_transposed_genotypes_joined_chr4.bed
```
```
$ sed -n '534,655p' maize_transposed_genotypes_joined_chr.bed > maize_transposed_genotypes_joined_chr5.bed
```
```
$ sed -n '656,731p' maize_transposed_genotypes_joined_chr.bed > maize_transposed_genotypes_joined_chr6.bed
```
```
$ sed -n '732,828p' maize_transposed_genotypes_joined_chr.bed > maize_transposed_genotypes_joined_chr7.bed
```
```
$ sed -n '829,890p' maize_transposed_genotypes_joined_chr.bed > maize_transposed_genotypes_joined_chr8.bed
```
```
$ sed -n '891,950p' maize_transposed_genotypes_joined_chr.bed > maize_transposed_genotypes_joined_chr9.bed
```
```
$ sed -n '951,956p' maize_transposed_genotypes_joined_chr.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_transposed_genotypes_joined_mutiple.bed
```
```
$ sed -n '957,983p' maize_transposed_genotypes_joined_chr.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_transposed_genotypes_joined_unknown.bed
```
```
$ sort -k4,4V maize_transposed_genotypes_joined_chr9.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr9_ordered_increased.bed 
```
### Order  based on increasing position values and with missing data encoded by this symbol: ?
```
$ sort -k4,4V maize_transposed_genotypes_joined_chr8.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr8_ordered_increased.bed
```
```
$ sort -k4,4V maize_transposed_genotypes_joined_chr7.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr7_ordered_increased.bed
```
```
$ sort -k4,4V maize_transposed_genotypes_joined_chr6.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr6_ordered_increased.bed
```
```
$ sort -k4,4V maize_transposed_genotypes_joined_chr5.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr5_ordered_increased.bed
```
```
$ sort -k4,4V maize_transposed_genotypes_joined_chr4.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr4_ordered_increased.bed
```
```
$ sort -k4,4V maize_transposed_genotypes_joined_chr3.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr3_ordered_increased.bed
```
```
$ sort -k4,4V maize_transposed_genotypes_joined_chr2.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr2_ordered_increased.bed
```
```
$ sort -k4,4V maize_transposed_genotypes_joined_chr1.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr1_ordered_increased.bed
```
```
$ sort -k4,4V maize_transposed_genotypes_joined_chr10.bed > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr10_ordered_increased.bed
```

decreasing position values and with missing data encoded by this symbol: -

```
$ sed 's/?/-/g' maize_transposed_genotypes_joined_chr8.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr8_ordered_decreased.bed
```
```
$ sed 's/?/-/g' maize_transposed_genotypes_joined_chr1.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr1_ordered_decreased.bed
```
```
$ sed 's/?/-/g' maize_transposed_genotypes_joined_chr2.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr2_ordered_decreased.bed
```
```
$ sed 's/?/-/g' maize_transposed_genotypes_joined_chr3.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr3_ordered_decreased.bed
```
```
$ sed 's/?/-/g' maize_transposed_genotypes_joined_chr4.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr4_ordered_decreased.bed
```
```
$ sed 's/?/-/g' maize_transposed_genotypes_joined_chr5.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr5_ordered_decreased.bed
```
```
$ sed 's/?/-/g' maize_transposed_genotypes_joined_chr6.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr6_ordered_decreased.bed
```
```
$ sed 's/?/-/g' maize_transposed_genotypes_joined_chr7.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr7_ordered_decreased.bed
```
```
$ sed 's/?/-/g' maize_transposed_genotypes_joined_chr9.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr9_ordered_decreased.bed
```
```
$ sed 's/?/-/g' maize_transposed_genotypes_joined_chr10.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/maize_chr10_ordered_decreased.bed
```
I joined (hint, hint) these data sets and put both genotypes and positions in a series of input files. 
For maize (Group = ZMMIL, ZMMLR, and ZMMMR in the third column of the fang_et_al_genotypes.txt file) we want 20 files in total:

10 files (1 for each chromosome) with SNPs ordered based on increasing position values and with missing data encoded by this symbol: ?

10 files (1 for each chromosome) with SNPs ordered based on decreasing position values and with missing data encoded by this symbol: -

1 file with all SNPs with unknown positions in the genome (these need not be ordered in any particular way)

1 file with all SNPs with multiple positions in the genome (these need not be ordered in any particular way)

For teosinte (Group = ZMPBA, ZMPIL, and ZMPJA in the third column of the fang_et_al_genotypes.txt file) we want 20 files in total:

10 files (1 for each chromosome) with SNPs ordered based on increasing position values and with missing data encoded by this symbol: ?

10 files (1 for each chromosome) with SNPs ordered based on decreasing position values and with missing data encoded by this symbol: -

1 file with all SNPs with unknown positions in the genome (these need not be ordered in any particular way)

1 file with all SNPs with multiple positions in the genome (these need not be ordered in any particular way)

A total of 44 files have been produced.




