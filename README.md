# LK-TEAM-Free-Fire-free-APIS
Free fire API

# 🔥 LK → TEAM | Free Fire API Suite (OB50) -- Some apis arent working for now🔥

Welcome to the **LK → TEAM Free Fire API Collection**, a powerful suite of endpoints built for Free Fire players, modders, and developers.  
Includes player stats, bio editing, nickname search, ban checking, JWT/token management, and more.  
> 🔄 Release: OB49 | 🟢 API Status: Online & Stable

---

## 📊 Player Info API

**Endpoint:**
```
https://info-ob49.vercel.app/api/account/?uid={uid}&region={region}
```

**Example:**
```
https://info-ob49.vercel.app/api/account/?uid=12345678&region=sg
```

**Response:**
```json
{
  "basicInfo": {
    "accountId": "12345678",
    "nickname": "FB:ㅤ@GMRemyX",
    "region": "SG",
    "level": 67,
    ...
  },
  "profileInfo": {
    "avatarId": 102000007,
    "equipedSkills": [204034042, 211037076, ...]
  },
  "clanBasicInfo": {
    "clanId": "60893361",
    "clanName": "MᴜᴍᴍʏEᴠᴀTᴇᴀᴍ",
    ...
  },
  "captainBasicInfo": { ... },
  "petInfo": {
    "name": "SiNo",
    "level": 7,
    ...
  },
  "socialInfo": {
    "signature": "FB & YT GM Remy | TikTok :gmremyx | IG GM Remy"
  },
  "diamondCostRes": {
    "diamondCost": 390
  },
  "creditScoreInfo": {
    "creditScore": 100
  }
}
```

---

## 🛑 Ban Check API

**Endpoint:**
```
https://lkteam-bancheck.deno.dev/checkban?uid={uid}
```

**Response:**
```json
{
  "uid": "12345678",
  "nickname": "FB:ㅤ@GMRemyX",
  "region": "SG",
  "banned": false,
  "ban_message": "Not banned",
  "ban_period_months": 0
}
```

---

## 🔐 Get Access Token

**Endpoint:**
```
https://grant-access-token.deno.dev/get_token?uid={guest_uid}&password={guest_password}
```

---

## 🛡️ Get JWT Token

**Endpoint:**
```
https://jwt-gen-api-v2.onrender.com/token?uid={guest_uid}&password={guest_password}
```

---

## ✏️ Change Bio API

**Endpoint:**
```
https://change-bio-api-lkteam.onrender.com/changebio?uid={uid}&password={password}&newbio={bio}&region={region}
```

**Example:**
```
https://change-bio-api-lkteam.onrender.com/changebio?uid=123&password=pass&newbio=[FF0000]LK[00FF00]TEAM&region=SG
```

---

## 👥 Send 100 Friend Requests

**Endpoint:**
```
https://spam-fr-lk-team.vercel.app/send_requests?uid={uid}
```

---

## 🔍 Search by Nickname API

**Endpoint:**
```
https://searchbynicknameapi.onrender.com/search?name={nickname}
```

**Example:**
```
https://searchbynicknameapi.onrender.com/search?name=xLK-TEAM-1
```

**Response:**
```json
{
  "result": [
    {
      "account_id": 12534439716,
      "nickname": "xLK-TEAM-1",
      "region": "NA",
      "level": 2
    },
    ...
  ]
}
```

---

## 🔁 Nickname Change API

**Endpoint:**
```
https://nickname-change-lkteam-dbww.onrender.com/change_nickname?jwt={jwt_token}&newname={new_name}
```

**Response:**
```json
{
  "account_id": 12496426251,
  "level": 2,
  "new_name": "LK-HYUN1",
  "old_name": "Room2T1F8Q9",
  "region": "TW",
  "status_code": 200
}
```

---

## 🔥 Likes API (V3)

**Endpoint:**
```
https://likes-api-lkteam-v3.onrender.com/like?uid={uid}&region={region}&count={count}
```

**Response:**
```json
{
  "failed_likes": 0,
  "level": 20,
  "likes_added": 97,
  "likes_after": 2686,
  "likes_before": 2589,
  "name": "Prince⁴⅝⁸⅚",
  "region": "US",
  "uid": "9067719977"
}
```

---

## 🤖 AI Ask API

**Endpoint:**
```
https://princeaiapi.vercel.app/prince/api/v1/ask?key=prince&ask={question}
```

---

## 👁️ Deep Search API

**Endpoint:**
```
https://lkai-deepsearch.deno.dev/deepsearch?q={query}&results={1-10}
```

---

## 🚀 Visits API

**Endpoint:**
```
https://lki-visits-api.deno.dev/{uid}
```

---

## ✅ Supported Regions

```
[ME, SG, BD, TH, VN, US, BR, SAC, NA]
```

## ❌ Unsupported Regions

```
[IND]
```

---

🧠 **Project by LK → TEAM**  
🎯 Focused on innovation, tools & automation for Free Fire community  
📩 Contact: Telegram `@lkteammm` | Discord: Coming soon...
