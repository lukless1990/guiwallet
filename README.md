**Install dependencies (only Ubuntu 16.04)**

```
wget http://humanitarycoin.org/install-dependencies.sh
bash install-dependencies.sh
```

**1. Clone wallet sources**

```
git clone https://github.com/humanitarycoin/guiwallet.git
```

**2. Modify `CryptoNoteWallet.cmake`**
 
```
set(CN_PROJECT_NAME "humanitarycoin")
set(CN_CURRENCY_DISPLAY_NAME "HumanitaryCoin")
set(CN_CURRENCY_TICKER "HCN")
```

**3. Clone HumanitaryCoin Source in guiwallet folder**

```
https://github.com/humanitarycoin/hcn.git
```

**3. Rename folder hcn to cryptonote**

```
mv hcn cryptonote
```

**5. Build**

```
mkdir build && cd build && cmake .. && make
```
