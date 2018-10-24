# Project X-Ray - Xilinx Series 7 Bitstream Documentation

[TOC]

This repo contains the bitstream documentation database for Xilinx Series 7
devices.

[HTML version of the Xilinx Series 7 BitStream is available on https://symbiflow.github.io/prjxray-db](https://symbiflow.github.io/prjxray-db).

This documentation was generated using the
[Project X-Ray tools](https://github.com/SymbiFlow/prjxray).

Due to the long time taken to create this database yourself, a prebuilt version
is currently being provided by Tim 'mithro' Ansell <<me@mith.ro>>. The database
is intended to kept in sync with the current prjxray output, but due to the
manual nature required to create it, it may sometimes lag behind
what you could create yourself using those tools.

Please try contacting [Tim](mailto:me@mith.ro) if you believe the database is
more than a week out of date.

# Contributions

As this repo is created from the prjxray output it doesn't accept external
contributions.  You are encourage to generate and maintain your own versions of
this documentation if your needs are not being met by this repository.

The
[htmlgen.py](https://github.com/SymbiFlow/prjxray/blob/master/htmlgen/htmlgen.py)
is kept in sync with the version in
[Project X-Ray](https://github.com/SymbiFlow/prjxray), please contribute all changes to
that file and then request Tim to rebuild the HTML output.

# License

These files are released under the very permissive [CC0 1.0 Universal](COPYING).

# Details

Last updated on Wed Oct 24 17:47:45 UTC 2018 (2018-10-24T17:47:45+00:00).

Created using [Project X-Ray](https://github.com/SymbiFlow/prjxray) version [v0.0-858-g7f2735d](https://github.com/SymbiFlow/prjxray/commit/7f2735dd4b5c9c695642b377515194af8909bf4d).

Latest commit was;
```
commit 7f2735dd4b5c9c695642b377515194af8909bf4d
Merge: 01c359c 47cc2b0
Author: Tim Ansell <me@mith.ro>
Date:   Tue Oct 23 09:57:25 2018 -0700

    Merge pull request #179 from litghost/fix_fuzzer
    
    Fix indirection.
```

## Database for [artix7](artix7/)

### Settings

Created using following [settings.sh (sha256: cb777c1e854d877556482ff2067eff348386ce627caa0ef5617a6e5dea01dc6a)](https://github.com/SymbiFlow/prjxray/blob/7f2735dd4b5c9c695642b377515194af8909bf4d/database/artix7/settings.sh)
```shell
export XRAY_DATABASE="artix7"
export XRAY_PART="xc7a50tfgg484-1"
export XRAY_ROI="SLICE_X12Y100:SLICE_X27Y149"
export XRAY_ROI_FRAMES="0x00000000:0xffffffff"

# Leave some CLBs to the left to allow easy ROI entering
export XRAY_ROI="SLICE_X8Y100:SLICE_X27Y149 RAMB18_X0Y40:RAMB18_X0Y59 RAMB36_X0Y20:RAMB36_X0Y29 DSP48_X0Y40:DSP48_X0Y59"
export XRAY_ROI_GRID_X1="18"
export XRAY_ROI_GRID_X2="47"
export XRAY_ROI_GRID_Y1="0"
export XRAY_ROI_GRID_Y2="52"

export XRAY_PIN_00="E22"
export XRAY_PIN_01="D22"
export XRAY_PIN_02="E21"
export XRAY_PIN_03="D21"
export XRAY_PIN_04="G21"
export XRAY_PIN_05="G22"
export XRAY_PIN_06="F21"

source $(dirname ${BASH_SOURCE[0]})/../../utils/environment.sh
```

### [Results](artix7/)

Results have checksums;

 * [`8c6097166bf4b43969c49894dc464d1202f19683d7287a63ec709bc867d97105  ./artix7/element_counts.csv`](./artix7/element_counts.csv)
 * [`6864d8edcef442cb129f83b9c5cd27be85d1b4bded8007bbeadcfc70717f8c48  ./artix7/gridinfo/grid-xc7a50tfgg484-1-db.txt`](./artix7/gridinfo/grid-xc7a50tfgg484-1-db.txt)
 * [`69f298082e6c8e537d8348b9d4c01f582d0d86fdeddf1e6606b90e800994bcdd  ./artix7/mask_bram_l.db`](./artix7/mask_bram_l.db)
 * [`8fae8a634efb8929db28581b2acd436fd4c31a0bd241dd4643e5692e2da8e648  ./artix7/mask_bram_r.db`](./artix7/mask_bram_r.db)
 * [`5c274320294201935a3edccb43eca8e347ca1f0acded71ec388c794877d4b55b  ./artix7/mask_clbll_l.db`](./artix7/mask_clbll_l.db)
 * [`5c274320294201935a3edccb43eca8e347ca1f0acded71ec388c794877d4b55b  ./artix7/mask_clbll_r.db`](./artix7/mask_clbll_r.db)
 * [`5c274320294201935a3edccb43eca8e347ca1f0acded71ec388c794877d4b55b  ./artix7/mask_clblm_l.db`](./artix7/mask_clblm_l.db)
 * [`5c274320294201935a3edccb43eca8e347ca1f0acded71ec388c794877d4b55b  ./artix7/mask_clblm_r.db`](./artix7/mask_clblm_r.db)
 * [`69f298082e6c8e537d8348b9d4c01f582d0d86fdeddf1e6606b90e800994bcdd  ./artix7/mask_dsp_l.db`](./artix7/mask_dsp_l.db)
 * [`8fae8a634efb8929db28581b2acd436fd4c31a0bd241dd4643e5692e2da8e648  ./artix7/mask_dsp_r.db`](./artix7/mask_dsp_r.db)
 * [`76d1e0bd4b7ad492cf3fe8698b2b5f46f7dcc5fe446984e5dccae373c63edafd  ./artix7/mask_hclk_l.db`](./artix7/mask_hclk_l.db)
 * [`76d1e0bd4b7ad492cf3fe8698b2b5f46f7dcc5fe446984e5dccae373c63edafd  ./artix7/mask_hclk_r.db`](./artix7/mask_hclk_r.db)
 * [`6baea72435613b87334f95cfe2b1ab36da4d57ada20b71a7dd870715b3e430c4  ./artix7/ppips_clbll_l.db`](./artix7/ppips_clbll_l.db)
 * [`3955d590e8ee64c843bb80f911a08781c1bac63e71b577436ae1f44195a88e22  ./artix7/ppips_clbll_r.db`](./artix7/ppips_clbll_r.db)
 * [`29f175153821dc13989eb580676ff0007e108d911275a74e7ebe45e819c14eaf  ./artix7/ppips_clblm_l.db`](./artix7/ppips_clblm_l.db)
 * [`52b53ae735d40632403283ab720db2172794a22c5245b3da7693b264d69a122d  ./artix7/ppips_clblm_r.db`](./artix7/ppips_clblm_r.db)
 * [`6d35b568a51f9b6761da2470a71738b2477ef72c16068a529ae8eb52b65bf17a  ./artix7/ppips_hclk_l.db`](./artix7/ppips_hclk_l.db)
 * [`81e0696179a33bdf8d2279a53b406911a403d50224355e9ad29eccee01a70305  ./artix7/ppips_hclk_r.db`](./artix7/ppips_hclk_r.db)
 * [`be617c15d1ec311b6249791414bbd69380fe90b476353cbb2fc2a7cb06f5029d  ./artix7/ppips_int_l.db`](./artix7/ppips_int_l.db)
 * [`a1423859c97a82dcfb114644f50b991db4ca7e0996e6d1ae4d2c97bfdfcb723d  ./artix7/ppips_int_r.db`](./artix7/ppips_int_r.db)
 * [`ce8aa28ad2ae2834d6182d6044cd0eae62da84551c486c1b04e3400116718f67  ./artix7/segbits_clbll_l.db`](./artix7/segbits_clbll_l.db)
 * [`087a5f7c98aa864b1a1232660806ecbd2f4fc1a963f387821ddab47d9c358d2c  ./artix7/segbits_clbll_r.db`](./artix7/segbits_clbll_r.db)
 * [`e2b4f7eda0ee7cc02db131660a9677e3264ab2ec2d1bdc833fa9218fbe62f97f  ./artix7/segbits_clblm_l.db`](./artix7/segbits_clblm_l.db)
 * [`d67044a5aeac20f746130c86c3a104fb7173f012325aeb181c19c9adaba3dbae  ./artix7/segbits_clblm_r.db`](./artix7/segbits_clblm_r.db)
 * [`20f7bf469951b04a56e5e140b6327470750b08960643353384b35baf85eb9117  ./artix7/segbits_hclk_l.db`](./artix7/segbits_hclk_l.db)
 * [`5e22f758a04eab3185b2453c9994aa2fa48f50ca8a6b49bf82e8fc4351f23a5c  ./artix7/segbits_hclk_r.db`](./artix7/segbits_hclk_r.db)
 * [`08dee581e565abbd09db559f9226139ba5a253f8aec4f3492152d8df8a87bbab  ./artix7/segbits_int_l.db`](./artix7/segbits_int_l.db)
 * [`be5f0c64ee17ad010dfea5125200216b2c69a558477a80133d043ed466e565be  ./artix7/segbits_int_r.db`](./artix7/segbits_int_r.db)
 * [`cb777c1e854d877556482ff2067eff348386ce627caa0ef5617a6e5dea01dc6a  ./artix7/settings.sh`](./artix7/settings.sh)
 * [`719d5ba5500fd77e2f07a161c67c6988999abdd7006db0187c8cbdcb04af44b8  ./artix7/site_type_BSCAN.json`](./artix7/site_type_BSCAN.json)
 * [`bb7ad365e043f69cbfcb943afb4943ccf732ea876ac8b07c926cb28007e65bbb  ./artix7/site_type_BUFGCTRL.json`](./artix7/site_type_BUFGCTRL.json)
 * [`a48f00785f54cbe2ca3ea567ceb02bf25d9d13fc868537ea8c720faf4331ad39  ./artix7/site_type_BUFHCE.json`](./artix7/site_type_BUFHCE.json)
 * [`6cb08677bcd99755d90f2df53630c3dc9c0b5d63c10c85aeef88a47ace492a93  ./artix7/site_type_BUFIO.json`](./artix7/site_type_BUFIO.json)
 * [`5688ee246f3f3e736e0c0b2d96e3338e72119f1584e4447d4a8fbfe19ad0290e  ./artix7/site_type_BUFMRCE.json`](./artix7/site_type_BUFMRCE.json)
 * [`dfdf5a8dba3a9e03a7c74baf3bf6cdedeb3b6284d1c602b51a8076c551f940c6  ./artix7/site_type_BUFR.json`](./artix7/site_type_BUFR.json)
 * [`a7b5800d4648666eaf72226199f1f7d4f93b2e69aa8d46e60883ea4b617f6d9e  ./artix7/site_type_CAPTURE.json`](./artix7/site_type_CAPTURE.json)
 * [`c78abb27787d2e81a93a5b264187a250f5ec035f004c09fa03858ed322f27886  ./artix7/site_type_DCIRESET.json`](./artix7/site_type_DCIRESET.json)
 * [`57a442cefa8bc14d804ba6694ca7a81e1b601f4acd30d9c0e90d5b4a9db9087a  ./artix7/site_type_DNA_PORT.json`](./artix7/site_type_DNA_PORT.json)
 * [`01bf735ad5e616c1e177edeb549f69b6f47e869af8d58ac5acf17ca715ea0475  ./artix7/site_type_DSP48E1.json`](./artix7/site_type_DSP48E1.json)
 * [`6eab82a31e033f73042853568f7d2b2c58574d1246393f6171a91796d00cb009  ./artix7/site_type_EFUSE_USR.json`](./artix7/site_type_EFUSE_USR.json)
 * [`942b9bda74fc803bbc3c2c4ca1f468018e14f323dd2222c8bcf9506c5b5d15e5  ./artix7/site_type_FIFO18E1.json`](./artix7/site_type_FIFO18E1.json)
 * [`e62595ccfb6649d74705597ed3dd6772a44f65c13f2ecc1fb4839c35f4b80662  ./artix7/site_type_FRAME_ECC.json`](./artix7/site_type_FRAME_ECC.json)
 * [`fc9aa800af2b598c9da95a1d0a7cd1aa368978954c67ada00d153dac2dba0870  ./artix7/site_type_GTPE2_CHANNEL.json`](./artix7/site_type_GTPE2_CHANNEL.json)
 * [`d0fe43e07827ac8662a939d79f23a975dffef400dc3a7308580c02352379e111  ./artix7/site_type_GTPE2_COMMON.json`](./artix7/site_type_GTPE2_COMMON.json)
 * [`23f8ebf5ab129a2d4a8dd2f2246e2ca963b969aa95a3d8cc3b2cbc581cdce035  ./artix7/site_type_IBUFDS_GTE2.json`](./artix7/site_type_IBUFDS_GTE2.json)
 * [`062968a37351ac566c60232cd5f618c145f76f2dca8fe16ba37dd05650ca9ec1  ./artix7/site_type_ICAP.json`](./artix7/site_type_ICAP.json)
 * [`f1c204574ca89912b1f2919aa7eda4fbedafacc44814612a3efcded392c194e2  ./artix7/site_type_IDELAYCTRL.json`](./artix7/site_type_IDELAYCTRL.json)
 * [`3e5a5a083444d1f0722a80ce21bb43e16606c3007aab7f441044c4aa1f1226a3  ./artix7/site_type_IDELAYE2.json`](./artix7/site_type_IDELAYE2.json)
 * [`c2886064c75316bff38b1aa03b60f24b1a646f96f918a2b9fbd2c1d904094f37  ./artix7/site_type_ILOGICE3.json`](./artix7/site_type_ILOGICE3.json)
 * [`e20dd0d79a5544f65c0064ab03c7647a6e187bfb94341f57e444593e9eafbc73  ./artix7/site_type_IN_FIFO.json`](./artix7/site_type_IN_FIFO.json)
 * [`449635c5afeb495eb1c0f80db8793d2414e06d84086e26cd545a707e74ea3575  ./artix7/site_type_IOB33.json`](./artix7/site_type_IOB33.json)
 * [`1368e7129596d2d28b513271c2b4c234a02135d98d0f7cdcc2d8b051561f1893  ./artix7/site_type_IOB33M.json`](./artix7/site_type_IOB33M.json)
 * [`62391d653ecf1901c6e1d5d287e7de3b10b83fd01ae087bacf6b66cf7454beb2  ./artix7/site_type_IOB33S.json`](./artix7/site_type_IOB33S.json)
 * [`2272f38176d4642a903727400d07f05b2e2f2789a446746d8cba0ce3efe46f74  ./artix7/site_type_IPAD.json`](./artix7/site_type_IPAD.json)
 * [`bd89171e213d5a48cb0b0b259f4d87c93e61f37ef91bb8cbcd36e1edba957c0f  ./artix7/site_type_MMCME2_ADV.json`](./artix7/site_type_MMCME2_ADV.json)
 * [`c46ad6bdb62ad4de869f99521322f8a770592752ed17930eb1cbfdfc65cf3b69  ./artix7/site_type_OLOGICE3.json`](./artix7/site_type_OLOGICE3.json)
 * [`b12f99c0eb9701d8995d421676c1699492ef88a155245a779be9569649c6617b  ./artix7/site_type_OPAD.json`](./artix7/site_type_OPAD.json)
 * [`97535aee9434b6b11a4f3d61ff3c0600206db0fc03ac8d75a9558f19c4fc8f5e  ./artix7/site_type_OUT_FIFO.json`](./artix7/site_type_OUT_FIFO.json)
 * [`b5f1988c0f167df0a2fdde664ed9a4fd8b6628c06e0e7fab9a1f5050eb4a466e  ./artix7/site_type_PCIE_2_1.json`](./artix7/site_type_PCIE_2_1.json)
 * [`47cec6b60c551a15721c6da588c14f3484be755d588f90d296ea7a11d04d46ba  ./artix7/site_type_PHASER_IN_PHY.json`](./artix7/site_type_PHASER_IN_PHY.json)
 * [`bb157302ba77dabd09614c88b959c9541150a0914b30c7a9c57f69d6c35d107b  ./artix7/site_type_PHASER_OUT_PHY.json`](./artix7/site_type_PHASER_OUT_PHY.json)
 * [`3b3b43e156ec1c4dc3c194eac174b87c2928a3ab28b3042cac446049610560b5  ./artix7/site_type_PHASER_REF.json`](./artix7/site_type_PHASER_REF.json)
 * [`e2c65ca031e4f50f1cc72ab519daeb8c0564efa6fee6a0c92969a7c945357358  ./artix7/site_type_PHY_CONTROL.json`](./artix7/site_type_PHY_CONTROL.json)
 * [`b1cfea0c3fc9a36a1ef6b3664af04d254aeb0a085ca2ae9ae8b84c104724ff27  ./artix7/site_type_PLLE2_ADV.json`](./artix7/site_type_PLLE2_ADV.json)
 * [`7641e6cbe65165dd0f67ce0ab1650a737683d37dde8c9aa798d665c99fc3d8c2  ./artix7/site_type_PMV2.json`](./artix7/site_type_PMV2.json)
 * [`3f8e9ada0f370ff1b40de2868064f7276fe73727fcfd6b725658ffbd57dcb8bf  ./artix7/site_type_RAMB18E1.json`](./artix7/site_type_RAMB18E1.json)
 * [`3aeb5f2a82ab0ed60295da343d05a4ca02f8d1774940b68659c495ec2de5daac  ./artix7/site_type_RAMBFIFO36E1.json`](./artix7/site_type_RAMBFIFO36E1.json)
 * [`1359e0ef3a2891cd173d9e8fd4306f445048484b4fb84acd83bd73b6be6a35d3  ./artix7/site_type_SLICEL.json`](./artix7/site_type_SLICEL.json)
 * [`93437b1d74625a1e627b5b9c20c1598e67fe4d265b218b8e8db6fdeac7f5345e  ./artix7/site_type_SLICEM.json`](./artix7/site_type_SLICEM.json)
 * [`69d0f7f4b92699b729766dcde4f2467c9d5d1f91093de2119729b295b91637d6  ./artix7/site_type_STARTUP.json`](./artix7/site_type_STARTUP.json)
 * [`1503bd8cd2bec47dd55ffad89ddc82e804dfd2c61e65c8770bc368ad7be9c8fa  ./artix7/site_type_TIEOFF.json`](./artix7/site_type_TIEOFF.json)
 * [`ac84a3db9159a0419d620dc2abb89e7f96de654239927a7400f9ed1fc41b977b  ./artix7/site_type_USR_ACCESS.json`](./artix7/site_type_USR_ACCESS.json)
 * [`78f4f1888dd814586b25e1008f59e0c0f094edeec8716e3acf962bc8ff13c9c1  ./artix7/site_type_XADC.json`](./artix7/site_type_XADC.json)
 * [`55bf341c1e05591dc68c29d5a4a3887ce7d7d83b1413d056ae31cbed5b2ceacf  ./artix7/tileconn.json`](./artix7/tileconn.json)
 * [`252a413af7d6bcc43aa55374acd45fbc5f15d1149a95b90494660d5581a88883  ./artix7/tilegrid.json`](./artix7/tilegrid.json)
 * [`fbf9a61be612301cff451f2838fda1331bd271f86e4ad7a46635443f0a864464  ./artix7/tile_type_BRAM_INT_INTERFACE_L.json`](./artix7/tile_type_BRAM_INT_INTERFACE_L.json)
 * [`9ecd392e781177913a73cc1fa7e45ceb5a9773948fe5d9f11835683dbb7b13ca  ./artix7/tile_type_BRAM_INT_INTERFACE_R.json`](./artix7/tile_type_BRAM_INT_INTERFACE_R.json)
 * [`c1d01ef9bfb2533b487b73bbbe0906990fea5640c7dadba04293c0b0074ff91b  ./artix7/tile_type_BRAM_L.json`](./artix7/tile_type_BRAM_L.json)
 * [`457e498e91bb77772a54d5a8afc666fcbd9a6e7a9acb32a3d5115c830afec5d7  ./artix7/tile_type_BRAM_R.json`](./artix7/tile_type_BRAM_R.json)
 * [`a13fddea8cd377ee4b783bead9ff50cac0e5801531c76607eb2ec66ecd6a67bb  ./artix7/tile_type_BRKH_BRAM.json`](./artix7/tile_type_BRKH_BRAM.json)
 * [`45c79e6fb0b495cff13416f6432904cdd01f470e751cfb4df1ef0ab6c2211e96  ./artix7/tile_type_BRKH_B_TERM_INT.json`](./artix7/tile_type_BRKH_B_TERM_INT.json)
 * [`56ec8fba5a5b60edfe4856ff0de807eff3133e47b04fba38598b8689512a14bc  ./artix7/tile_type_BRKH_CLB.json`](./artix7/tile_type_BRKH_CLB.json)
 * [`23bfbe9b4c732c6d51898cd73e8b4973fe283e6a34596663be7f1eafb17cd55d  ./artix7/tile_type_BRKH_CLK.json`](./artix7/tile_type_BRKH_CLK.json)
 * [`c392b0992733376bca89170108f25bc519cd06b1c2a7728a587851ec10a31b9c  ./artix7/tile_type_BRKH_CMT.json`](./artix7/tile_type_BRKH_CMT.json)
 * [`053b695a0caa573d233e594e05b8de80eb9811b1b9449aa7727d29d985003217  ./artix7/tile_type_BRKH_DSP_L.json`](./artix7/tile_type_BRKH_DSP_L.json)
 * [`086e76a9b644fde9f16830a0cc8c2e69b0e5ceacc3bff301e296cab6e46def5d  ./artix7/tile_type_BRKH_DSP_R.json`](./artix7/tile_type_BRKH_DSP_R.json)
 * [`cd3292cd07e35176dbefb646091d16baaaec74c736bc1adb843a0190f51d24af  ./artix7/tile_type_BRKH_GTX.json`](./artix7/tile_type_BRKH_GTX.json)
 * [`783d3d6baa2d053c918135919f638b5ff32e2b6e6c8a08efaea319456b8f0a7e  ./artix7/tile_type_BRKH_INT.json`](./artix7/tile_type_BRKH_INT.json)
 * [`8da1c4f26f810b32ad36183bfaf4d297c0bba54654dbdf0598d1dbb567689738  ./artix7/tile_type_BRKH_TERM_INT.json`](./artix7/tile_type_BRKH_TERM_INT.json)
 * [`bba1dbca008dd4848a28786bf4615f3c1c808bf6cf954b1d9361e071cfb79927  ./artix7/tile_type_B_TERM_INT.json`](./artix7/tile_type_B_TERM_INT.json)
 * [`0a3cddc74a5e6ab37cf4a7c1deaf523b70d31fe321575f3f41eb1178cb72b69b  ./artix7/tile_type_CFG_CENTER_BOT.json`](./artix7/tile_type_CFG_CENTER_BOT.json)
 * [`701d86922f2e283b19d3aec708dfc2d2943b765f910e106388d6ec5ea2ae4d80  ./artix7/tile_type_CFG_CENTER_MID.json`](./artix7/tile_type_CFG_CENTER_MID.json)
 * [`500c4949209a249f8998c1ca28c51f55995b5d8bbba6875806368e3b4dc68e83  ./artix7/tile_type_CFG_CENTER_TOP.json`](./artix7/tile_type_CFG_CENTER_TOP.json)
 * [`af4b4675ea714d3b7518297d2a4075dc8fdfb3fcc651b12b4f742b2cd6f46445  ./artix7/tile_type_CLBLL_L.json`](./artix7/tile_type_CLBLL_L.json)
 * [`3dc18dec76cf080a3ab430eeeb966308565025f8144f9032e312fa51a8947020  ./artix7/tile_type_CLBLL_R.json`](./artix7/tile_type_CLBLL_R.json)
 * [`73426d37d590fadbdb25d65eecfaf5ac9940f9722d115a22cfb87282fd6eddf8  ./artix7/tile_type_CLBLM_L.json`](./artix7/tile_type_CLBLM_L.json)
 * [`2c033c3a5bece3055e38144c3897c8a55a83a1a344ec432aa77e6f751c9e75b1  ./artix7/tile_type_CLBLM_R.json`](./artix7/tile_type_CLBLM_R.json)
 * [`587d08841fdde19107be139169b561d120974f9092f741b37eabe5ddea15b641  ./artix7/tile_type_CLK_BUFG_BOT_R.json`](./artix7/tile_type_CLK_BUFG_BOT_R.json)
 * [`de8913143bf5b996e57d02d75710b7372a761d4f900036a75b03496797cee9e4  ./artix7/tile_type_CLK_BUFG_REBUF.json`](./artix7/tile_type_CLK_BUFG_REBUF.json)
 * [`6c6693b97f6d461b9815e05fc7a20b0b00fb3c19301711be04226496057a204b  ./artix7/tile_type_CLK_BUFG_TOP_R.json`](./artix7/tile_type_CLK_BUFG_TOP_R.json)
 * [`c9532a45b785d3533e2033969e029f13062ecc42b805c0d2b23ee218ceab45eb  ./artix7/tile_type_CLK_FEED.json`](./artix7/tile_type_CLK_FEED.json)
 * [`1c632ab0754f6227a8dbafd07a0e02bda0911cabd245dce22b78ff4e02645d36  ./artix7/tile_type_CLK_HROW_BOT_R.json`](./artix7/tile_type_CLK_HROW_BOT_R.json)
 * [`be9d7e276eae46e1610b0dc43e15c94d2f62eb6621841de19193322faf7f965d  ./artix7/tile_type_CLK_HROW_TOP_R.json`](./artix7/tile_type_CLK_HROW_TOP_R.json)
 * [`70c631e800c0cc9805008ce98ef6cf24f39adc6a52609f3cf60a6779b0e6cedf  ./artix7/tile_type_CLK_MTBF2.json`](./artix7/tile_type_CLK_MTBF2.json)
 * [`43951c358c372eec561ab8c85bc32a2fb587b12aae11df3ff267b63f35737e9a  ./artix7/tile_type_CLK_PMV2.json`](./artix7/tile_type_CLK_PMV2.json)
 * [`9e20005e5e7f408baf72be5dc81afb67a955025a7dcf326e0cdb55c7998c5c0b  ./artix7/tile_type_CLK_PMV2_SVT.json`](./artix7/tile_type_CLK_PMV2_SVT.json)
 * [`906947ad12479e10b27b425aec2436dea8805ea450c51b1078292db31b864408  ./artix7/tile_type_CLK_PMVIOB.json`](./artix7/tile_type_CLK_PMVIOB.json)
 * [`20375dee2190e4fd7c14649ed1b8d3530f77707b55384f91f2653765591927ef  ./artix7/tile_type_CLK_PMV.json`](./artix7/tile_type_CLK_PMV.json)
 * [`73efe99e80904057c04de32e440cb43ded9c650c7df7bd60d5c0a0a33763a8e8  ./artix7/tile_type_CLK_TERM.json`](./artix7/tile_type_CLK_TERM.json)
 * [`506844d8f2ba25985a75da70b91923e8291185b378db5e519ce3b6f9796888b6  ./artix7/tile_type_CMT_FIFO_L.json`](./artix7/tile_type_CMT_FIFO_L.json)
 * [`372e0e8c12570745bb871ba1a3af507e5a2ec7221a2737d6bf25ff81b42062a5  ./artix7/tile_type_CMT_FIFO_R.json`](./artix7/tile_type_CMT_FIFO_R.json)
 * [`a8c3d0926852c2d75ed88ac4da930b1deb1a388f7bbe7c7c2d32b2ca8cf85d27  ./artix7/tile_type_CMT_PMV.json`](./artix7/tile_type_CMT_PMV.json)
 * [`11804b256e364ae6fe0c2df27b84b266f50287516d47824f5dc8a43a8dc93f7c  ./artix7/tile_type_CMT_PMV_L.json`](./artix7/tile_type_CMT_PMV_L.json)
 * [`c8115d9218adc87294f5adc8215a3364ec85e24b391b4bf75d0045b85568226d  ./artix7/tile_type_CMT_TOP_L_LOWER_B.json`](./artix7/tile_type_CMT_TOP_L_LOWER_B.json)
 * [`25fe320f8407a75982acc46a025676f27a6be2efaa34e5770adb52a9241ed95f  ./artix7/tile_type_CMT_TOP_L_LOWER_T.json`](./artix7/tile_type_CMT_TOP_L_LOWER_T.json)
 * [`2071d7876faa386a2ac1ad94d972893818f94db4170f8c4c05b0af8de695f8f3  ./artix7/tile_type_CMT_TOP_L_UPPER_B.json`](./artix7/tile_type_CMT_TOP_L_UPPER_B.json)
 * [`9b8d21d151f144632cb718416d9ec5407f712e8940b65495d1a72b1beb80f0c8  ./artix7/tile_type_CMT_TOP_L_UPPER_T.json`](./artix7/tile_type_CMT_TOP_L_UPPER_T.json)
 * [`84c14df1c55d309511cedd7fcd613a282cd303fc02094b9dcae4c57c0c9954ab  ./artix7/tile_type_CMT_TOP_R_LOWER_B.json`](./artix7/tile_type_CMT_TOP_R_LOWER_B.json)
 * [`179a16f60b86284ce8d527c29e305ac4ad9173b0017e5e5ac4921eea3543ebd4  ./artix7/tile_type_CMT_TOP_R_LOWER_T.json`](./artix7/tile_type_CMT_TOP_R_LOWER_T.json)
 * [`801471c567005d6a9bcf9d3ff721e25971059f0436339d89e470c659b2d7b16f  ./artix7/tile_type_CMT_TOP_R_UPPER_B.json`](./artix7/tile_type_CMT_TOP_R_UPPER_B.json)
 * [`753feebf0d24ba3b1e758035842cbb1a064b4de3e16e8cb95df829031beee92f  ./artix7/tile_type_CMT_TOP_R_UPPER_T.json`](./artix7/tile_type_CMT_TOP_R_UPPER_T.json)
 * [`f2d9f69bd40843d8344bc13d5aefd5ddbb76dc71627711b821e57e8fa43bbcbb  ./artix7/tile_type_DSP_L.json`](./artix7/tile_type_DSP_L.json)
 * [`542e02a3773906f1094c2a6bc4aa2ac4a722abf29952ecd2d32d56960c09146c  ./artix7/tile_type_DSP_R.json`](./artix7/tile_type_DSP_R.json)
 * [`a62a62d9154122081360f5dd3d0663ff6117e76983ed15fe7907f549cbe3478e  ./artix7/tile_type_GTP_CHANNEL_0.json`](./artix7/tile_type_GTP_CHANNEL_0.json)
 * [`58ef6c05c0a1bb99cced08583946c485273bb68bf4af5f3c3d7f0644e573ec79  ./artix7/tile_type_GTP_CHANNEL_1.json`](./artix7/tile_type_GTP_CHANNEL_1.json)
 * [`6c5f62d5baf00bab7c75b0ffe6d95329a67c9b9b3385bb5e26fa213a190153be  ./artix7/tile_type_GTP_CHANNEL_2.json`](./artix7/tile_type_GTP_CHANNEL_2.json)
 * [`9fee55da6f1f89e69f10caa41a536727f1be944dd44e8f5c544a35666f20efe6  ./artix7/tile_type_GTP_CHANNEL_3.json`](./artix7/tile_type_GTP_CHANNEL_3.json)
 * [`b9cffc2e886d5dee8f23e48c9c983f7d9935f34df8dd3d2a18a32b592554c2e6  ./artix7/tile_type_GTP_COMMON.json`](./artix7/tile_type_GTP_COMMON.json)
 * [`c528ad2c4bc67e0aba5bc2f0e1428647beb687ae3adfa77bfc70a34a29fc0388  ./artix7/tile_type_GTP_INT_INTERFACE.json`](./artix7/tile_type_GTP_INT_INTERFACE.json)
 * [`26f90d4bf3ae82c8ce379f512ae0268c55fc704b5c6c8598c53956b91529572b  ./artix7/tile_type_HCLK_BRAM.json`](./artix7/tile_type_HCLK_BRAM.json)
 * [`3bdf08d4f43e8a9dc2bc12851f8e38e51413c9ec0683f420937498eed45aafc6  ./artix7/tile_type_HCLK_CLB.json`](./artix7/tile_type_HCLK_CLB.json)
 * [`c78dd2e261f0a5fc6eafd71c8003205dbed53de9ed7a5742ca246b22047b55b0  ./artix7/tile_type_HCLK_CMT.json`](./artix7/tile_type_HCLK_CMT.json)
 * [`109b67fe5bbbcd6268fb86fed4764c912d15f77c9ddc430e8a228bf73ec00bfe  ./artix7/tile_type_HCLK_CMT_L.json`](./artix7/tile_type_HCLK_CMT_L.json)
 * [`5be1593662a6e1ec359df098ba71caa5f108309424cc11117339854f56a1c33c  ./artix7/tile_type_HCLK_DSP_L.json`](./artix7/tile_type_HCLK_DSP_L.json)
 * [`85c6b7ac250bbeb1fe16926c0b9fe3ebde3abc150c95c68e07dcb0edb54b967f  ./artix7/tile_type_HCLK_DSP_R.json`](./artix7/tile_type_HCLK_DSP_R.json)
 * [`3e31fcf205a9c67f5a24be910469e8b8760514278d13750dc999fe32c77edfad  ./artix7/tile_type_HCLK_FEEDTHRU_1.json`](./artix7/tile_type_HCLK_FEEDTHRU_1.json)
 * [`5d07288892cd1a21f8523e3c685ca2ac0247bf8271805b002a2787636049254c  ./artix7/tile_type_HCLK_FEEDTHRU_2.json`](./artix7/tile_type_HCLK_FEEDTHRU_2.json)
 * [`7df47db37e12f3784ab35c17380d080d274deca72e9d34fe6df62b759d42dcd2  ./artix7/tile_type_HCLK_FIFO_L.json`](./artix7/tile_type_HCLK_FIFO_L.json)
 * [`fa3811fac61d8faa25a02abf59c1f503742564810bd017881dd7d5761e518b96  ./artix7/tile_type_HCLK_GTX.json`](./artix7/tile_type_HCLK_GTX.json)
 * [`1de429f755bfb2eea7d5baa133a878909ad14cfda5110ab09ae0a6d981d15930  ./artix7/tile_type_HCLK_INT_INTERFACE.json`](./artix7/tile_type_HCLK_INT_INTERFACE.json)
 * [`4eebe24c98614a1790dca73de5d59df9ce584e9fa83f2dfdf65e45687f8ea408  ./artix7/tile_type_HCLK_IOB.json`](./artix7/tile_type_HCLK_IOB.json)
 * [`440a6be2c50ad4e65da67d6d562eaa94c9d5d39515f680812b69de893a7b3ae8  ./artix7/tile_type_HCLK_IOI3.json`](./artix7/tile_type_HCLK_IOI3.json)
 * [`8d52c10eef9c998da9f580947259e8870fc03a78c1c4576de55f374b20400a06  ./artix7/tile_type_HCLK_L_BOT_UTURN.json`](./artix7/tile_type_HCLK_L_BOT_UTURN.json)
 * [`2dd453008337e840b6000776e01e6492774e233f1c6a229a564d43b0b40e7c90  ./artix7/tile_type_HCLK_L.json`](./artix7/tile_type_HCLK_L.json)
 * [`ec18789fe138cb9a7f55092e7454008f448f61ff6114374761223514a3141a5c  ./artix7/tile_type_HCLK_R_BOT_UTURN.json`](./artix7/tile_type_HCLK_R_BOT_UTURN.json)
 * [`0ff88dcc12f1174afbb9762d5f9a51c94b1f48e9fce7a2e270612f49a778fdd7  ./artix7/tile_type_HCLK_R.json`](./artix7/tile_type_HCLK_R.json)
 * [`35d4e6f1829f4f8caa20144b93747f7413e2c3b2ed98b0bf10af41158bf81f46  ./artix7/tile_type_HCLK_TERM_GTX.json`](./artix7/tile_type_HCLK_TERM_GTX.json)
 * [`c7f8b5def602269f1897e40d1c3ac9b0b12c5b7a544bd3f309e710154719c321  ./artix7/tile_type_HCLK_TERM.json`](./artix7/tile_type_HCLK_TERM.json)
 * [`33d48102d07627a90a0d45cde55180cd54a41c4221d8000a3086116b5e163076  ./artix7/tile_type_HCLK_VBRK.json`](./artix7/tile_type_HCLK_VBRK.json)
 * [`ad0f50a03faa49e02dbc39600861e3c353a490e22f1334f8ab774bc1bd3ad4c0  ./artix7/tile_type_HCLK_VFRAME.json`](./artix7/tile_type_HCLK_VFRAME.json)
 * [`cc895f8d7eb437df6282b7c1eca5ceb157fbac7a95b1fd1c93fa65621cd112ca  ./artix7/tile_type_INT_FEEDTHRU_1.json`](./artix7/tile_type_INT_FEEDTHRU_1.json)
 * [`12ad58aa01c4a2399ebf2b49c334c06188341ddd3aee0d7f79f44228a74ae94c  ./artix7/tile_type_INT_FEEDTHRU_2.json`](./artix7/tile_type_INT_FEEDTHRU_2.json)
 * [`c0921f4040358b3ccc5205e54c788448d751c0c130dfadcf23a843f4508503d0  ./artix7/tile_type_INT_INTERFACE_L.json`](./artix7/tile_type_INT_INTERFACE_L.json)
 * [`86dc9518591ed0dd2e2c61e9b2d50e6da3ee4d2d684472f7429001bcbcbda2bb  ./artix7/tile_type_INT_INTERFACE_R.json`](./artix7/tile_type_INT_INTERFACE_R.json)
 * [`3dcb7f202b74d980159e2de40257d5098e6f900477d06297f80990b0e9155751  ./artix7/tile_type_INT_L.json`](./artix7/tile_type_INT_L.json)
 * [`b4e4f309fe6917bb52b4661a53e9ea8bd6a192cd6cb65bb4bd9cca898d16cf55  ./artix7/tile_type_INT_R.json`](./artix7/tile_type_INT_R.json)
 * [`9dab8290edf106109e221c7e759ae45d3050b8d5e9574f7bf5058361e3ae4e2a  ./artix7/tile_type_IO_INT_INTERFACE_L.json`](./artix7/tile_type_IO_INT_INTERFACE_L.json)
 * [`87f6ae714d73ec34eaae4f4d3299c5048b29b9ecdc9b9a025101af7c8ea4bd38  ./artix7/tile_type_IO_INT_INTERFACE_R.json`](./artix7/tile_type_IO_INT_INTERFACE_R.json)
 * [`b2f0206eea59366caf11ac3431a8677fb31def9541a465f8215fce9e31a4cdf2  ./artix7/tile_type_LIOB33.json`](./artix7/tile_type_LIOB33.json)
 * [`6a4b98bd6ba5778c8f01e0d809f605e549f225a040f0a679b8e1b4bc5760c3f6  ./artix7/tile_type_LIOB33_SING.json`](./artix7/tile_type_LIOB33_SING.json)
 * [`a9afa4ac21293b465e15ec1cf3957882a42bf79a00880c34e5e2922cc213b670  ./artix7/tile_type_LIOI3.json`](./artix7/tile_type_LIOI3.json)
 * [`1989a5d335af8e857dfdbcdfa3d1ebae142f467f115b1534ba4279d6f8289c04  ./artix7/tile_type_LIOI3_SING.json`](./artix7/tile_type_LIOI3_SING.json)
 * [`b6e2459db179551ddb5667c88aace86b5b1ebc15d25e9ed16e5f3a1a89eb8b7c  ./artix7/tile_type_LIOI3_TBYTESRC.json`](./artix7/tile_type_LIOI3_TBYTESRC.json)
 * [`8479bc74592125bb6f90c9c0006ebf0a8cc95c81800dd7ba7149c4c80d91d101  ./artix7/tile_type_LIOI3_TBYTETERM.json`](./artix7/tile_type_LIOI3_TBYTETERM.json)
 * [`10376bfc02f7c4e7510c81a3e8aa24aca76eeab6c036ed25e9a1165da7b6dec9  ./artix7/tile_type_L_TERM_INT.json`](./artix7/tile_type_L_TERM_INT.json)
 * [`0bac0a1dab6df6c11cf9b4a91272d32c25fd0ab52d5ec7318eceed7efafedf94  ./artix7/tile_type_MONITOR_BOT.json`](./artix7/tile_type_MONITOR_BOT.json)
 * [`2cd0b749aad9258f7bee31812865ac916833a2d70a5bafd4cbee93aedf046bff  ./artix7/tile_type_MONITOR_MID.json`](./artix7/tile_type_MONITOR_MID.json)
 * [`9a3ff3040e1641921d333a3572425429a26594385d2712b76aef329e31bb9111  ./artix7/tile_type_MONITOR_TOP.json`](./artix7/tile_type_MONITOR_TOP.json)
 * [`cc31a014f02a5118f0b055e9ef23cab3f6e594b2bfecde17286d7a597217ce2b  ./artix7/tile_type_NULL.json`](./artix7/tile_type_NULL.json)
 * [`f41f1a2e33f92a90e14b1f3ef2f73a370cc9beece5708ae39348a8a29b4129f2  ./artix7/tile_type_PCIE_BOT.json`](./artix7/tile_type_PCIE_BOT.json)
 * [`51d5eaf8ebe162275f3c1fbbe0b29c04a87ce2b2568ba2b8a7613d3ce7409d63  ./artix7/tile_type_PCIE_INT_INTERFACE_L.json`](./artix7/tile_type_PCIE_INT_INTERFACE_L.json)
 * [`498ee4fe83ed42161359e341123128a12c300c73b257b538603c549307088f0c  ./artix7/tile_type_PCIE_INT_INTERFACE_R.json`](./artix7/tile_type_PCIE_INT_INTERFACE_R.json)
 * [`06bda788813b1db788f628323d6b8ca59171dc7e64fb63af9ffa01a012867e7c  ./artix7/tile_type_PCIE_NULL.json`](./artix7/tile_type_PCIE_NULL.json)
 * [`d78c4e54abf9825b87f078b8ba873a2a557fb10da98a2eea7655da41eb5f78d5  ./artix7/tile_type_PCIE_TOP.json`](./artix7/tile_type_PCIE_TOP.json)
 * [`7c0d7c33e3202c5f7dba96ad45f1fc2fc3908ceaac81a567e2fe3e0523ebb288  ./artix7/tile_type_RIOB33.json`](./artix7/tile_type_RIOB33.json)
 * [`cf4f1facf67039f411e2a1ea6ad6cedf78fdb38aad748b50cfc229e814361f47  ./artix7/tile_type_RIOB33_SING.json`](./artix7/tile_type_RIOB33_SING.json)
 * [`e74e663259e2ea679e77899b5344759c30a68e01f5a51af1ca491ad28d33e302  ./artix7/tile_type_RIOI3.json`](./artix7/tile_type_RIOI3.json)
 * [`3ad139c28fe8f7251fb921ca178d4ca56ea6e0ed9a3aad7f41a31b32aac8358c  ./artix7/tile_type_RIOI3_SING.json`](./artix7/tile_type_RIOI3_SING.json)
 * [`a301f932092e5475755a8dd15e0eb5e505d698d54b8bd04516ffff970d0ebc44  ./artix7/tile_type_RIOI3_TBYTESRC.json`](./artix7/tile_type_RIOI3_TBYTESRC.json)
 * [`622609c9fa4398e276da3c0153e2dbc2a681d1c0f9268039aad416b85cbd217e  ./artix7/tile_type_RIOI3_TBYTETERM.json`](./artix7/tile_type_RIOI3_TBYTETERM.json)
 * [`25e056ead534be2890f05d39c946f1db3e0e946575c9e263e67c58491be6c1a3  ./artix7/tile_type_R_TERM_INT_GTX.json`](./artix7/tile_type_R_TERM_INT_GTX.json)
 * [`52e4abec4c0fa0b0fb41f12b10490a0876ae2ab537223eb5421fdd8881fdf7ec  ./artix7/tile_type_R_TERM_INT.json`](./artix7/tile_type_R_TERM_INT.json)
 * [`0716e74334b122441a5181a3520071fabed24c8d2b9ffe9516a211757dd9be98  ./artix7/tile_type_TERM_CMT.json`](./artix7/tile_type_TERM_CMT.json)
 * [`2de0186436eaff3618b63a1b4da63cb2433b252f64b0d39114abf85a8d5f9440  ./artix7/tile_type_T_TERM_INT.json`](./artix7/tile_type_T_TERM_INT.json)
 * [`af19906dbd78dd5c685994cfec1858eccbc324063fd8f4a60c208deecb615419  ./artix7/tile_type_VBRK_EXT.json`](./artix7/tile_type_VBRK_EXT.json)
 * [`b97c56f95ae1334f6bd2b7f8cb5782b0f6e335c8c34260555ff31dd0a165bb47  ./artix7/tile_type_VBRK.json`](./artix7/tile_type_VBRK.json)
 * [`b24c32758a7c21185e2b9689b4ac65f8f00e43e8ec46aac79a8233b3d3fd36c6  ./artix7/tile_type_VFRAME.json`](./artix7/tile_type_VFRAME.json)
 * [`ef0724733da87455426a0f833642d96e9d206d047f4eb97072c3093f80c40d7d  ./artix7/xc7a35tcpg236-1.yaml`](./artix7/xc7a35tcpg236-1.yaml)
 * [`41c360b1e2f7e08b9051f1160a34954ce4c05a445a07f226f1f4059caf1fa1d3  ./artix7/xc7a50tfgg484-1.yaml`](./artix7/xc7a50tfgg484-1.yaml)

## Database for [kintex7](kintex7/)

### Settings

Created using following [settings.sh (sha256: 2daf6a69dd6d20df7b1273ff43c5c340abe36f8229d297646865edcfd91eff18)](https://github.com/SymbiFlow/prjxray/blob/7f2735dd4b5c9c695642b377515194af8909bf4d/database/kintex7/settings.sh)
```shell
export XRAY_DATABASE="kintex7"
export XRAY_PART="xc7k70tfbg676-2"
export XRAY_ROI="SLICE_X0Y50:SLICE_X19Y99 DSP48_X0Y20:DSP48_X0Y39 RAMB18_X0Y20:RAMB18_X0Y39 RAMB36_X0Y10:RAMB36_X0Y19"
export XRAY_ROI_FRAMES="0x00400100:0x004006ff"
export XRAY_ROI_GRID_X1="9"
export XRAY_ROI_GRID_X2="38"
export XRAY_ROI_GRID_Y1="104"
export XRAY_ROI_GRID_Y2="156"
# Choose the first N High Range I/Os
export XRAY_PIN_00="K25"
export XRAY_PIN_01="K26"
export XRAY_PIN_02="L24"
export XRAY_PIN_03="L25"
export XRAY_PIN_04="M19"
export XRAY_PIN_05="M20"
export XRAY_PIN_06="M21"

source $(dirname ${BASH_SOURCE[0]})/../../utils/environment.sh
```

### [Results](kintex7/)

Results have checksums;

 * [`6f6dd0ba33fdd78d87f8591adbff5aad2d3653a1b1fa03d77079ce64a7c1f175  ./kintex7/mask_bram0_l.db`](./kintex7/mask_bram0_l.db)
 * [`9d12bc3be758587479874bff531ad702f429a963518d7bc5b2b3c0400ded4c6a  ./kintex7/mask_bram0_r.db`](./kintex7/mask_bram0_r.db)
 * [`6f6dd0ba33fdd78d87f8591adbff5aad2d3653a1b1fa03d77079ce64a7c1f175  ./kintex7/mask_bram1_l.db`](./kintex7/mask_bram1_l.db)
 * [`9d12bc3be758587479874bff531ad702f429a963518d7bc5b2b3c0400ded4c6a  ./kintex7/mask_bram1_r.db`](./kintex7/mask_bram1_r.db)
 * [`6f6dd0ba33fdd78d87f8591adbff5aad2d3653a1b1fa03d77079ce64a7c1f175  ./kintex7/mask_bram2_l.db`](./kintex7/mask_bram2_l.db)
 * [`9d12bc3be758587479874bff531ad702f429a963518d7bc5b2b3c0400ded4c6a  ./kintex7/mask_bram2_r.db`](./kintex7/mask_bram2_r.db)
 * [`6f6dd0ba33fdd78d87f8591adbff5aad2d3653a1b1fa03d77079ce64a7c1f175  ./kintex7/mask_bram3_l.db`](./kintex7/mask_bram3_l.db)
 * [`9d12bc3be758587479874bff531ad702f429a963518d7bc5b2b3c0400ded4c6a  ./kintex7/mask_bram3_r.db`](./kintex7/mask_bram3_r.db)
 * [`6f6dd0ba33fdd78d87f8591adbff5aad2d3653a1b1fa03d77079ce64a7c1f175  ./kintex7/mask_bram4_l.db`](./kintex7/mask_bram4_l.db)
 * [`9d12bc3be758587479874bff531ad702f429a963518d7bc5b2b3c0400ded4c6a  ./kintex7/mask_bram4_r.db`](./kintex7/mask_bram4_r.db)
 * [`03fe7af3125c25f3d84bd8e874525c83275a6c3b6736d0b01134b5f982721f5b  ./kintex7/mask_clbll_l.db`](./kintex7/mask_clbll_l.db)
 * [`be34841c9aa64527e5f84d1819abbac1d324047367003b6fdc1402cd695481de  ./kintex7/mask_clbll_r.db`](./kintex7/mask_clbll_r.db)
 * [`fec2e4a94efd8b4e9d29d52689d406482f842e6f718ab671131b5e9ac2e0805b  ./kintex7/mask_clblm_l.db`](./kintex7/mask_clblm_l.db)
 * [`7b68fbcb19382d54bdc57971dd7eb9b0cbb4318f9b6053b301f3384f7ee4bb75  ./kintex7/mask_clblm_r.db`](./kintex7/mask_clblm_r.db)
 * [`6f6dd0ba33fdd78d87f8591adbff5aad2d3653a1b1fa03d77079ce64a7c1f175  ./kintex7/mask_dsp0_l.db`](./kintex7/mask_dsp0_l.db)
 * [`9d12bc3be758587479874bff531ad702f429a963518d7bc5b2b3c0400ded4c6a  ./kintex7/mask_dsp0_r.db`](./kintex7/mask_dsp0_r.db)
 * [`6f6dd0ba33fdd78d87f8591adbff5aad2d3653a1b1fa03d77079ce64a7c1f175  ./kintex7/mask_dsp1_l.db`](./kintex7/mask_dsp1_l.db)
 * [`9d12bc3be758587479874bff531ad702f429a963518d7bc5b2b3c0400ded4c6a  ./kintex7/mask_dsp1_r.db`](./kintex7/mask_dsp1_r.db)
 * [`6f6dd0ba33fdd78d87f8591adbff5aad2d3653a1b1fa03d77079ce64a7c1f175  ./kintex7/mask_dsp2_l.db`](./kintex7/mask_dsp2_l.db)
 * [`9d12bc3be758587479874bff531ad702f429a963518d7bc5b2b3c0400ded4c6a  ./kintex7/mask_dsp2_r.db`](./kintex7/mask_dsp2_r.db)
 * [`6f6dd0ba33fdd78d87f8591adbff5aad2d3653a1b1fa03d77079ce64a7c1f175  ./kintex7/mask_dsp3_l.db`](./kintex7/mask_dsp3_l.db)
 * [`9d12bc3be758587479874bff531ad702f429a963518d7bc5b2b3c0400ded4c6a  ./kintex7/mask_dsp3_r.db`](./kintex7/mask_dsp3_r.db)
 * [`6f6dd0ba33fdd78d87f8591adbff5aad2d3653a1b1fa03d77079ce64a7c1f175  ./kintex7/mask_dsp4_l.db`](./kintex7/mask_dsp4_l.db)
 * [`9d12bc3be758587479874bff531ad702f429a963518d7bc5b2b3c0400ded4c6a  ./kintex7/mask_dsp4_r.db`](./kintex7/mask_dsp4_r.db)
 * [`3e3b19a2d49a1d0f25937bc5d0b33f0269c22c5e8ae3cfe52e4ff5c65843b134  ./kintex7/segbits_clbll_l.db`](./kintex7/segbits_clbll_l.db)
 * [`fdb5499b9e2aa9d1796332279f0b5dc881a5ad0796698e8ef3af40ddc98df26b  ./kintex7/segbits_clbll_r.db`](./kintex7/segbits_clbll_r.db)
 * [`0b79670cc5a03b7580f73dc162a8bad048ade2f50971622138e0d0a5759899b6  ./kintex7/segbits_clblm_l.db`](./kintex7/segbits_clblm_l.db)
 * [`e7f5d16940fde9397f69d5f52c2a6339641191dc9dba4466e8b7f9e5f6a735bf  ./kintex7/segbits_clblm_r.db`](./kintex7/segbits_clblm_r.db)
 * [`9ed8769618df03902c73e78312467108c7b74b903ac61d1bbbba1fd9710e6d3b  ./kintex7/segbits_int_l.db`](./kintex7/segbits_int_l.db)
 * [`dbf6cba5bbba95d7d78d9b51d236d8819dc776c2ebc540521e5b48d3a2c1390f  ./kintex7/segbits_int_r.db`](./kintex7/segbits_int_r.db)
 * [`2daf6a69dd6d20df7b1273ff43c5c340abe36f8229d297646865edcfd91eff18  ./kintex7/settings.sh`](./kintex7/settings.sh)
 * [`8f5b7a7924adec5132208cf8e851e81bcb01a5c61f8839eb5a5de0b20b924510  ./kintex7/tilegrid.json`](./kintex7/tilegrid.json)
 * [`68426295ab4a35e367c9dff93e4f9b807afd43fe83418cb2da7465cd4d7177a2  ./kintex7/xc7k70tfbg676-2.yaml`](./kintex7/xc7k70tfbg676-2.yaml)
