# 📐 Subnet Host Calculation in IPv4

## 🧮 Formula to Calculate Number of Usable Hosts

- `32` is the total number of bits in an IPv4 address.
- Subtract `2` to exclude:
  - 1 for the **network address**
  - 1 for the **broadcast address**

---

## 📊 Examples of CIDR to Host Calculations

| CIDR | Subnet Mask       | Host Bits | Total Hosts | Usable Hosts |
|------|-------------------|-----------|-------------|--------------|
| /30  | 255.255.255.252   | 2         | 4           | 2            |
| /29  | 255.255.255.248   | 3         | 8           | 6            |
| /28  | 255.255.255.240   | 4         | 16          | 14           |
| /27  | 255.255.255.224   | 5         | 32          | 30           |
| /26  | 255.255.255.192   | 6         | 64          | 62           |
| /25  | 255.255.255.128   | 7         | 128         | 126          |
| /24  | 255.255.255.0     | 8         | 256         | 254          |
| /23  | 255.255.254.0     | 9         | 512         | 510          |
| /22  | 255.255.252.0     | 10        | 1024        | 1022         |
| /21  | 255.255.248.0     | 11        | 2048        | 2046         |
| /20  | 255.255.240.0     | 12        | 4096        | 4094         |
| /16  | 255.255.0.0       | 16        | 65,536      | 65,534       |
| /8   | 255.0.0.0         | 24        | 16,777,216  | 16,777,214   |

---

## 🧠 Example: Calculate Hosts in `192.168.1.0/26`

- Subnet prefix: `/26`
- Host bits = `32 - 26 = 6`
- Total addresses = `2^6 = 64`
- **Usable hosts = 64 - 2 = 62**

---

## ✅ Summary

- Use the formula: `(2^(32 - subnet bits)) - 2`
- Subtract `2` for network & broadcast addresses
- Larger subnet prefix = fewer usable hosts

# 🧮 How to Find the Subnet Mask from CIDR

CIDR (e.g., `/24`) represents the number of bits used for the **network portion** of an IP address.

## 🔄 Conversion Steps

### 1. **Determine the number of network bits**  
The number after the `/` tells you how many bits are set to `1` in the subnet mask.

Example: `/24` → first 24 bits are `1`s.

---

### 2. **Convert to Binary Subnet Mask**
Break the 32-bit binary into 4 octets:

- `/24` → 24 ones followed by 8 zeros  
  → `11111111.11111111.11111111.00000000`

---

### 3. **Convert Each Octet to Decimal**

| Binary Octet     | Decimal |
|------------------|---------|
| `11111111`       | 255     |
| `11111111`       | 255     |
| `11111111`       | 255     |
| `00000000`       | 0       |

So, `/24` → **255.255.255.0**

---

## 🧪 CIDR to Subnet Mask Chart

| CIDR | Subnet Mask         |
|------|----------------------|
| /8   | 255.0.0.0            |
| /16  | 255.255.0.0          |
| /24  | 255.255.255.0        |
| /25  | 255.255.255.128      |
| /26  | 255.255.255.192      |
| /27  | 255.255.255.224      |
| /28  | 255.255.255.240      |
| /29  | 255.255.255.248      |
| /30  | 255.255.255.252      |
| /31  | 255.255.255.254      |
| /32  | 255.255.255.255      |

---

## 🧠 Example: Convert `/26` to Subnet Mask

- `/26` → 26 bits of `1`, 6 bits of `0`
- Binary: `11111111.11111111.11111111.11000000`
- Decimal: `255.255.255.192`

✅ `/26` = **255.255.255.192**

---

## ✅ Summary

To find the subnet mask from CIDR:
- Use the number after `/` to set that many bits to `1`
- Convert to 4-octet binary
- Translate each octet to decimal

