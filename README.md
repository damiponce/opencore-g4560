# OpenCore 0.7.8 
Tested on macOS Monterey 12.2.1

## System specifications
| Part | Model |
| :--- | :--- |
| MB | Gigabyte GA-H110M-H (r1.0) |
| CPU | Intel Pentium G4560 |
| dGPU | ASUS Radeon RX 550 2GB (Lexa) |
| RAM | 4GB @ 2133 MHz <br/> 8GB @ 2400 MHz |
| HDD | WD Blue 1TB |

![image](https://user-images.githubusercontent.com/10394094/154425589-79ba5b70-5671-440c-a8c9-c03677498ffb.png)


## NOTES
- Hardware acceleration works thanks to SSTD-GPU-SPOOF (taken from [this user's EFI folder](https://www.tonymacx86.com/threads/success-big-sur-10-11-4-ga-z170n-wifi-samsung-860-evo-rx550.313767/)), even though the Lexa architecture isn't supported, only Baffin.
- Haven't tried the iGPU but it wouldn't have HW accel anyways because it's a Pentium.
- Also haven't tried power delivery optimizations yet, I'm not sure how much extra  performance could that bring me. 
- ALSO also, no USB mapping done since I didn't find it necessary yet.
- You can probably remove the contents of the Audio folder (`EFI > OC > Resources > Audio`) if you're tight with space in your boot partition.
