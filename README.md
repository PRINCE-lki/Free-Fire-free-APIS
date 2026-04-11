# 🔥 Free Fire Info API

> 🎮 Unofficial Free Fire Player Information & Statistics API

```
Base URL: https://freefireinfo-zy9l.onrender.com
API Version: v1
```

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Authentication](#-authentication)
- [Endpoints](#-endpoints)
  - [Search Players](#-search-players)
  - [Player Stats](#-player-stats)
  - [Player Profile](#-player-profile)
- [Supported Regions](#-supported-regions)
- [Rate Limits](#-rate-limits)
- [Error Handling](#-error-handling)
- [Usage Examples](#-usage-examples)
- [Credits & Attribution](#-credits--attribution)
- [Disclaimer](#-disclaimer)

---

## 🌟 Overview

The **Free Fire Info API** provides developers with programmatic access to Free Fire player data, including search functionality, detailed statistics, and comprehensive profile information. This API is designed for building gaming tools, stat trackers, and community applications.

> ⚠️ **Note:** This is an unofficial API. It is not affiliated with or endorsed by Garena Free Fire.

---

## ✨ Features

- 🔍 **Player Search**: Find players by username or keyword across multiple regions
- 📊 **Detailed Statistics**: Retrieve Battle Royale and Clash Squad mode stats
- 👤 **Profile Information**: Access comprehensive player profiles with optional gallery, blacklist, and spark data
- 🌍 **Multi-Region Support**: Query players across 13+ Free Fire server regions
- 🔄 **Flexible Parameters**: Customize responses with optional query parameters

---

## 🔐 Authentication

> Currently, this API instance does **not require authentication** for public endpoints. However, rate limiting may apply.

```http
# No API key required for basic usage
GET /api/v1/search-players?keyword=PlayerName
```

---

## 📡 Endpoints

### 🔍 Search Players

Search for Free Fire players by username or keyword.

```http
GET /api/v1/search-players
```

#### Parameters

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `keyword` | string | ✅ Yes | Search term (minimum 3 characters) |
| `server` | string | ❌ No | Server region (default: `IND`) |

#### Supported Server Values
```
IND, SG, RU, ID, TW, US, VN, TH, ME, PK, CIS, BR, BD
```

#### Example Request
```bash
curl "https://freefireinfo-zy9l.onrender.com/api/v1/search-players?keyword=LKTEAM&server=US"
```

#### Example Response
```json
{
  "infos": [
    {
      "accountid": "3049658523",
      "accounttype": 1,
      "nickname": "LKTEAM\n⚡",
      "region": "BR",
      "level": 18,
      "exp": 18276,
      "bannerid": 901000345,
      "rank": 301,
      "rankingpoints": 1000,
      "badgeid": 1001000095,
      "seasonid": 50,
      "liked": 91,
      "lastloginat": "1619674580",
      "csrank": 301,
      "maxrank": 301,
      "csmaxrank": 301,
      "externaliconinfo": {
        "status": "EXTERNALICONSTATUSNOTINUSE",
        "showtype": "EXTERNALICONSHOWTYPEFRIEND"
      },
      "hipporank": 1,
      "hipporankingpoints": 1
    },
    {
      "accountid": "7167328380",
      "accounttype": 1,
      "nickname": "LKTEAM ‽ Rp",
      "region": "BR",
      "level": 6,
      "exp": 2546,
      "headpic": 902000006,
      "rank": 301,
      "rankingpoints": 1000,
      "badgeid": 1001000095,
      "seasonid": 50,
      "liked": 16,
      "lastloginat": "1671141526",
      "csrank": 301,
      "maxrank": 301,
      "csmaxrank": 301,
      "externaliconinfo": {
        "status": "EXTERNALICONSTATUSNOTINUSE",
        "showtype": "EXTERNALICONSHOWTYPEFRIEND"
      },
      "hipporank": 1,
      "hipporankingpoints": 1
    },
    {
      "accountid": "4570314056",
      "accounttype": 1,
      "nickname": "LKTEAM JB",
      "region": "BR",
      "level": 6,
      "exp": 1904,
      "rank": 301,
      "rankingpoints": 1000,
      "badgeid": 1001000095,
      "seasonid": 50,
      "liked": 2,
      "lastloginat": "1638987604",
      "csrank": 301,
      "maxrank": 301,
      "csmaxrank": 301,
      "externaliconinfo": {
        "status": "EXTERNALICONSTATUSNOTINUSE",
        "showtype": "EXTERNALICONSHOWTYPEFRIEND"
      },
      "hipporank": 1,
      "hipporankingpoints": 1
    },
    {
      "accountid": "4570130943",
      "accounttype": 1,
      "nickname": "LKTEAM JB YT",
      "region": "BR",
      "level": 6,
      "exp": 1859,
      "rank": 301,
      "rankingpoints": 1000,
      "badgeid": 1001000095,
      "seasonid": 50,
      "liked": 1,
      "lastloginat": "1639147162",
      "csrank": 301,
      "maxrank": 301,
      "csmaxrank": 301,
      "externaliconinfo": {
        "status": "EXTERNALICONSTATUSNOTINUSE",
        "showtype": "EXTERNALICONSHOWTYPEFRIEND"
      },
      "hipporank": 1,
      "hipporankingpoints": 1
    },
    {
      "accountid": "7577993003",
      "accounttype": 1,
      "nickname": "lkteam^^",
      "region": "BR",
      "level": 3,
      "exp": 327,
      "rank": 301,
      "rankingpoints": 1000,
      "badgeid": 1001000095,
      "seasonid": 50,
      "lastloginat": "1680746518",
      "csrank": 301,
      "maxrank": 301,
      "csmaxrank": 301,
      "externaliconinfo": {
        "status": "EXTERNALICONSTATUSNOTINUSE",
        "showtype": "EXTERNALICONSHOWTYPEFRIEND"
      },
      "hipporank": 1,
      "hipporankingpoints": 1
    },
    {
      "accountid": "7637149114",
      "accounttype": 1,
      "nickname": "LKTEAM^^.^:^",
      "region": "BR",
      "level": 3,
      "exp": 441,
      "headpic": 902000007,
      "rank": 301,
      "rankingpoints": 1000,
      "badgeid": 1001000095,
      "seasonid": 50,
      "liked": 1,
      "lastloginat": "1681977489",
      "csrank": 301,
      "maxrank": 301,
      "csmaxrank": 301,
      "externaliconinfo": {
        "status": "EXTERNALICONSTATUSNOTINUSE",
        "showtype": "EXTERNALICONSHOWTYPEFRIEND"
      },
      "hipporank": 1,
      "hipporankingpoints": 1
    },
    {
      "accountid": "3095785435",
      "accounttype": 1,
      "nickname": "LKTEAM_",
      "region": "BR",
      "level": 2,
      "exp": 174,
      "rank": 301,
      "rankingpoints": 1000,
      "badgeid": 1001000095,
      "seasonid": 50,
      "lastloginat": "1620145009",
      "csrank": 301,
      "maxrank": 301,
      "csmaxrank": 301,
      "externaliconinfo": {
        "status": "EXTERNALICONSTATUSNOTINUSE",
        "showtype": "EXTERNALICONSHOWTYPEFRIEND"
      },
      "hipporank": 1,
      "hipporankingpoints": 1
    },
    {
      "accountid": "3170190113",
      "accounttype": 1,
      "nickname": "LKteam__",
      "region": "BR",
      "level": 4,
      "exp": 664,
      "rank": 301,
      "rankingpoints": 1000,
      "badgeid": 1001000095,
      "seasonid": 50,
      "lastloginat": "1621383776",
      "csrank": 301,
      "maxrank": 301,
      "csmaxrank": 301,
      "externaliconinfo": {
        "status": "EXTERNALICONSTATUSNOTINUSE",
        "showtype": "EXTERNALICONSHOWTYPEFRIEND"
      },
      "hipporank": 1,
      "hipporankingpoints": 1
    },
    {
      "accountid": "6676168866",
      "accounttype": 1,
      "nickname": "LKTEAM__✓",
      "region": "BR",
      "level": 10,
      "exp": 6635,
      "rank": 301,
      "rankingpoints": 1000,
      "badgeid": 1001000095,
      "seasonid": 50,
      "liked": 22,
      "lastloginat": "1661931446",
      "csrank": 301,
      "maxrank": 301,
      "csmaxrank": 301,
      "externaliconinfo": {
        "status": "EXTERNALICONSTATUSNOTINUSE",
        "showtype": "EXTERNALICONSHOWTYPEFRIEND"
      },
      "hipporank": 1,
      "hipporankingpoints": 1
    },
    {
      "accountid": "7059962061",
      "accounttype": 1,
      "nickname": "LKTEAM__BB",
      "region": "BR",
      "level": 3,
      "exp": 457,
      "rank": 301,
      "rankingpoints": 1000,
      "badgeid": 1001000095,
      "seasonid": 50,
      "lastloginat": "1668073014",
      "csrank": 301,
      "maxrank": 301,
      "csmaxrank": 301,
      "externaliconinfo": {
        "status": "EXTERNALICONSTATUSNOTINUSE",
        "showtype": "EXTERNALICONSHOWTYPEFRIEND"
      },
      "hipporank": 1,
      "hipporankingpoints": 1
    }
  ]
}
```

---

### 📊 Player Stats

Retrieve detailed statistics for a specific player including Battle Royale and Clash Squad modes.

```http
GET /api/v1/player-stats
```

#### Parameters

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `uid` | string | ✅ Yes | Player UID (numeric value) |
| `server` | string | ❌ No | Server region (default: `IND`) |
| `gamemode` | string | ❌ No | Game mode: `'br'` or `'cs'` (default: `br`) |
| `matchmode` | string | ❌ No | Match type: `'CAREER'`, `'NORMAL'`, or `'RANKED'` (default: `CAREER`) |

#### Example Request
```bash
curl "https://freefireinfo-zy9l.onrender.com/api/v1/player-stats?uid=907719977&server=US&gamemode=br&matchmode=CARREER"
```

#### Example Response
```json
{
  "data": {
    "duostats": {
      "accountid": "9067719977",
      "detailedstats": {
        "damage": 13117,
        "deaths": 15,
        "distanceTravelled": 55655,
        "headshotKills": 13,
        "headshots": 41,
        "highestKills": 16,
        "knockDown": 41,
        "pickUps": 941,
        "survivalTime": 4699,
        "topNTimes": 3
      },
      "gamesplayed": 16,
      "kills": 42,
      "wins": 1
    },
    "quadstats": {
      "accountid": "9067719977",
      "detailedstats": {
        "damage": 43202,
        "deaths": 31,
        "distanceTravelled": 152914,
        "headshotKills": 30,
        "headshots": 98,
        "highestKills": 18,
        "knockDown": 99,
        "pickUps": 3000,
        "revives": 2,
        "survivalTime": 16361,
        "topNTimes": 9
      },
      "gamesplayed": 37,
      "kills": 101,
      "wins": 6
    },
    "solostats": {
      "accountid": "9067719977",
      "detailedstats": {
        "damage": 107291,
        "deaths": 55,
        "distanceTravelled": 307169,
        "headshotKills": 150,
        "headshots": 326,
        "highestKills": 29,
        "pickUps": 7336,
        "survivalTime": 34681,
        "topNTimes": 36
      },
      "gamesplayed": 73,
      "kills": 462,
      "wins": 18
    }
  },
  "metadata": {
    "gamemode": "br",
    "matchmode": "CAREER",
    "server": "US",
    "uid": "9067719977"
  },
  "success": true
}
```

---

### 👤 Player Profile

Get comprehensive player profile information including gallery, blacklist status, and spark info.

```http
GET /api/v1/player-profile
```

#### Parameters

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `uid` | string | ✅ Yes | Player UID (positive integer) |
| `server` | string | ❌ No | Server region (default: `IND`) |
| `need_gallery_info` | boolean | ❌ No | Include gallery information (default: `false`) |
| `need_blacklist` | boolean | ❌ No | Include blacklist status (default: `false`) |
| `need_spark_info` | boolean | ❌ No | Include spark info (default: `false`) |
| `call_sign_src` | integer | ❌ No | Call sign source (default: `7`) |

#### Example Request
```bash
curl "https://freefireinfo-zy9l.onrender.com/api/v1/player-profile?uid=1234567890&need_gallery_info=true&need_blacklist=true"
```

#### Example Response
```json
{
  "basicinfo": {
    "accountid": "9067719977",
    "accounttype": 1,
    "nickname": "PRINCEㅤ:(ㅤ:(",
    "region": "US",
    "level": 37,
    "exp": 88663,
    "bannerid": 901052004,
    "headpic": 902052026,
    "rank": 309,
    "rankingpoints": 1920,
    "badgecnt": 8,
    "badgeid": 1001000095,
    "seasonid": 50,
    "liked": 6486,
    "showrank": true,
    "lastloginat": "1775932250",
    "csrank": 311,
    "csrankingpoints": 41,
    "weaponskinshows": [
      912052001
    ],
    "maxrank": 309,
    "csmaxrank": 311,
    "accountprefers": {
      "csPeakPregameShowChoices": [
        1
      ]
    },
    "createat": "1711419920",
    "title": 904090015,
    "externaliconinfo": {
      "status": "EXTERNALICONSTATUSNOTINUSE",
      "showtype": "EXTERNALICONSHOWTYPEFRIEND"
    },
    "releaseversion": "OB53",
    "showbrrank": true,
    "showcsrank": true,
    "socialhighlightswithbasicinfo": {},
    "itemtaginfo": [
      {}
    ],
    "hipporank": 9,
    "hipporankingpoints": 11
  },
  "profileinfo": {
    "avatarid": 102000007,
    "clothes": [
      50
    ],
    "equipedskills": [
      214000000,
      204052002,
      211052001,
      203052002,
      205052002
    ],
    "pveprimaryweapon": 1,
    "endtime": 1,
    "ismarkedstar": true
  },
  "historyepinfo": [
    {
      "epeventid": 94,
      "epbadge": 1001000094,
      "badgecnt": 36,
      "bpicon": "UI_BP_Emoji_Treasure26",
      "maxlevel": 100,
      "eventname": "T_52_SH_BP94_NAME"
    },
    {
      "epeventid": 93,
      "epbadge": 1001000093,
      "badgecnt": 108,
      "bpicon": "UI_BP_Emoji_Pisces",
      "maxlevel": 100,
      "eventname": "T_52_SH_BP93_NAME"
    },
    {
      "epeventid": 92,
      "epbadge": 1001000092,
      "badgecnt": 127,
      "bpicon": "UI_BP_Emoji_Redhat25",
      "maxlevel": 100,
      "eventname": "T_51_SH_BP92_NAME"
    },
    {
      "epeventid": 91,
      "epbadge": 1001000091,
      "badgecnt": 85,
      "bpicon": "UI_BP_Emoji_Sagittarius25",
      "maxlevel": 100,
      "eventname": "T_51_SH_BP91_NAME"
    },
    {
      "epeventid": 90,
      "epbadge": 1001000090,
      "badgecnt": 25,
      "bpicon": "UI_BP_Emoji_Ghost25",
      "maxlevel": 100,
      "eventname": "T_51_SH_BP90_NAME"
    },
    {
      "epeventid": 89,
      "epbadge": 1001000089,
      "badgecnt": 44,
      "bpicon": "UI_BP_Emoji_Cloudyday",
      "maxlevel": 100,
      "eventname": "T_50_SH_BP89_NAME"
    },
    {
      "epeventid": 88,
      "epbadge": 1001000088,
      "badgecnt": 14,
      "bpicon": "UI_BP_Emoji_Dunelord",
      "maxlevel": 100,
      "eventname": "T_50_SH_BP88_NAME"
    },
    {
      "epeventid": 87,
      "epbadge": 1001000087,
      "badgecnt": 17,
      "bpicon": "UI_BP_Emoji_Funzombie",
      "maxlevel": 100,
      "eventname": "T_50_SH_BP87_NAME"
    },
    {
      "epeventid": 86,
      "epbadge": 1001000086,
      "badgecnt": 59,
      "bpicon": "UI_BP_Emoji_TvMan",
      "maxlevel": 100,
      "eventname": "T_49_SH_BP86_NAME"
    },
    {
      "epeventid": 85,
      "epbadge": 1001000085,
      "badgecnt": 1,
      "bpicon": "UI_BP_Emoji_Sparta",
      "maxlevel": 100,
      "eventname": "T_49_SH_BP85_NAME"
    },
    {
      "epeventid": 84,
      "epbadge": 1001000084,
      "badgecnt": 4,
      "bpicon": "UI_BP_Emoji_Cupnoodle",
      "maxlevel": 100,
      "eventname": "T_48_H_BP84_NAME"
    },
    {
      "epeventid": 83,
      "epbadge": 1001000083,
      "badgecnt": 1,
      "bpicon": "UI_BP_Emoji_Firefly",
      "maxlevel": 100,
      "eventname": "T_48_H_BP83_NAME"
    },
    {
      "epeventid": 82,
      "epbadge": 1001000082,
      "badgecnt": 11,
      "bpicon": "UI_BP_Emoji_Comic24",
      "maxlevel": 100,
      "eventname": "T_48_H_BP82_NAME"
    },
    {
      "epeventid": 81,
      "epbadge": 1001000081,
      "badgecnt": 9,
      "bpicon": "UI_BP_Emoji_Express",
      "maxlevel": 100,
      "eventname": "T_47_H_BP81_NAME"
    },
    {
      "epeventid": 80,
      "epbadge": 1001000080,
      "badgecnt": 38,
      "bpicon": "UI_BP_Emoji_Tailor",
      "maxlevel": 100,
      "eventname": "T_47_H_BP80_NAME"
    },
    {
      "epeventid": 79,
      "epbadge": 1001000079,
      "badgecnt": 29,
      "bpicon": "UI_BP_Emoji_Pinata",
      "maxlevel": 100,
      "eventname": "T_46_H_BP79_NAME"
    },
    {
      "epeventid": 78,
      "epbadge": 1001000078,
      "badgecnt": 57,
      "bpicon": "UI_BP_Emoji_DingDing",
      "maxlevel": 100,
      "eventname": "T_46_H_BP78_NAME"
    },
    {
      "epeventid": 77,
      "epbadge": 1001000077,
      "badgecnt": 19,
      "bpicon": "UI_BP_Emoji_Smile",
      "maxlevel": 100,
      "eventname": "T_46_H_BP77_NAME"
    },
    {
      "epeventid": 76,
      "epbadge": 1001000076,
      "badgecnt": 17,
      "bpicon": "UI_BP_Emoji_Octopus",
      "maxlevel": 100,
      "eventname": "T_45_H_BP76_NAME"
    },
    {
      "epeventid": 75,
      "epbadge": 1001000075,
      "badgecnt": 24,
      "bpicon": "UI_BP_Emoji_Leo",
      "maxlevel": 100,
      "eventname": "T_45_H_BP75_NAME"
    },
    {
      "epeventid": 74,
      "epbadge": 1001000074,
      "badgecnt": 9,
      "bpicon": "UI_BP_Emoji_Goose",
      "maxlevel": 100,
      "eventname": "T_45_H_BP74_NAME"
    },
    {
      "epeventid": 73,
      "epbadge": 1001000073,
      "badgecnt": 8,
      "bpicon": "UI_BP_Emoji_Fragment",
      "maxlevel": 100,
      "eventname": "T_44_H_BP73_NAME"
    },
    {
      "epeventid": 72,
      "epbadge": 1001000072,
      "badgecnt": 26,
      "bpicon": "UI_BP_Emoji_Videogame",
      "maxlevel": 100,
      "eventname": "T_44_H_BP72_NAME"
    },
    {
      "epeventid": 71,
      "epbadge": 1001000071,
      "badgecnt": 6,
      "bpicon": "UI_BP_Emoji_Pointed",
      "maxlevel": 100,
      "eventname": "T_43_H_BP71_NAME"
    },
    {
      "epeventid": 70,
      "epbadge": 1001000070,
      "badgecnt": 2,
      "bpicon": "UI_BP_Emoji_Frog",
      "maxlevel": 100,
      "eventname": "T_43_H_BP70_NAME"
    }
  ],
  "clanbasicinfo": {
    "clanid": "2050879926",
    "clanname": "WGSV",
    "captainid": "4828986870",
    "clanlevel": 1,
    "capacity": 25,
    "membernum": 8
  },
  "captainbasicinfo": {
    "accountid": "4828986870",
    "accounttype": 1,
    "nickname": "꧁ԝɪ⍳⍳ɪᴀᴍ₄ₖ꧂",
    "region": "US",
    "level": 61,
    "exp": 1171707,
    "bannerid": 901046014,
    "headpic": 902046036,
    "rank": 319,
    "rankingpoints": 3272,
    "badgecnt": 23,
    "badgeid": 1001000095,
    "seasonid": 50,
    "liked": 2219,
    "showrank": true,
    "lastloginat": "1775705469",
    "csrank": 308,
    "csrankingpoints": 29,
    "pinid": 910000004,
    "maxrank": 319,
    "csmaxrank": 308,
    "accountprefers": {
      "csPeakPregameShowChoices": [
        1
      ]
    },
    "createat": "1640974789",
    "title": 904090024,
    "externaliconinfo": {
      "status": "EXTERNALICONSTATUSNOTINUSE",
      "showtype": "EXTERNALICONSHOWTYPEFRIEND"
    },
    "releaseversion": "OB53",
    "showbrrank": true,
    "showcsrank": true,
    "socialhighlightswithbasicinfo": {},
    "hipporank": 18,
    "hipporankingpoints": 8
  },
  "petinfo": {
    "id": 1300000125,
    "level": 4,
    "exp": 540,
    "isselected": true,
    "skinid": 1310000257,
    "selectedskillid": 1315000018
  },
  "socialinfo": {
    "accountid": "9067719977",
    "gender": "GENDERMALE",
    "language": "LANGUAGETURKISH",
    "timeactive": "TIMEACTIVENIGHT",
    "modeprefer": "MODEPREFERENTERTAINMENT",
    "signature": "THE BEST...",
    "rankshow": "RANKSHOWCS"
  },
  "diamondcostres": {
    "diamondcost": 800
  },
  "creditscoreinfo": {
    "creditscore": 100,
    "rewardstate": "REWARDSTATEUNCLAIMED",
    "periodicsummaryendtime": "1775932186",
    "periodicsummarylevel": 1776191386
  },
  "userSparkInfo": {
    "state": "SparkState_EXTINGUISHED",
    "level": 32100
  }
}
```

---

## 🌍 Supported Regions

| Code | Region | Code | Region |
|------|--------|------|--------|
| `IND` | India | `SG` | Singapore |
| `RU` | Russia | `ID` | Indonesia |
| `TW` | Taiwan | `US` | North America |
| `VN` | Vietnam | `TH` | Thailand |
| `ME` | Middle East | `PK` | Pakistan |
| `CIS` | CIS | `BR` | Brazil |
| `BD` | Bangladesh | | |

---

## ⚡ Rate Limits

> 📌 Rate limiting policies may vary. Please implement exponential backoff in your applications.

- **Recommended**: Max 60 requests/minute per IP
- **Burst**: Up to 10 requests/second allowed

---

## ❌ Error Handling

All errors return standard HTTP status codes with JSON response bodies.

#### Common Status Codes

| Code | Meaning | Description |
|------|---------|-------------|
| `200` | OK | Request succeeded |
| `400` | Bad Request | Invalid parameters |
| `404` | Not Found | Player or endpoint not found |
| `429` | Too Many Requests | Rate limit exceeded |
| `500` | Server Error | Internal server error |

#### Error Response Format
```json
{
  "status": "error",
  "code": 404,
  "message": "Player not found"
}
```

---

## 💻 Usage Examples

### JavaScript (Fetch API)
```javascript
async function searchPlayer(keyword, server = 'IND') {
  const response = await fetch(
    `https://freefireinfo-zy9l.onrender.com/api/v1/search-players?keyword=${keyword}&server=${server}`
  );
  const data = await response.json();
  return data;
}

// Usage
searchPlayer('ProGamer', 'SG').then(console.log);
```

### Python (Requests)
```python
import requests

def get_player_stats(uid, server='IND', gamemode='br'):
    url = "https://freefireinfo-zy9l.onrender.com/api/v1/player-stats"
    params = {'uid': uid, 'server': server, 'gamemode': gamemode}
    response = requests.get(url, params=params)
    return response.json()

# Usage
stats = get_player_stats('1234567890', server='SG')
print(stats)
```

### cURL
```bash
# Search for a player
curl "https://freefireinfo-zy9l.onrender.com/api/v1/search-players?keyword=Elite&server=BR"

# Get player stats
curl "https://freefireinfo-zy9l.onrender.com/api/v1/player-stats?uid=9876543210&gamemode=cs"

# Get full profile with optional data
curl "https://freefireinfo-zy9l.onrender.com/api/v1/player-profile?uid=9876543210&need_gallery_info=true&need_spark_info=true"
```

---

## 🎨 Credits & Attribution

### 👑 Primary Credits

> This API documentation and service is powered by the amazing work of **LK_TEAM**.

```
╔════════════════════════════════════╗
║  🔥 LK → TEAM 🔥                   ║
║  Free Fire API Suite               ║
║                                    ║
║  🧠 Project by: LK → TEAM          ║
║  🎯 Focus: Innovation & Tools      ║
║  📩 Contact: Telegram @lkteammm    ║
╚════════════════════════════════════╝
```

### 🔗 Related Projects by LK-TEAM

- [PRINCE-LKTEAM/Free-Fire-API](https://github.com/PRINCE-LKTEAM/Free-Fire-API) [[3]]
- [PRINCE-lki/Free-Fire-free-APIS](https://github.com/PRINCE-lki/Free-Fire-free-APIS) [[11]]

### 🙏 Acknowledgements

- **LK-TEAM** for developing and maintaining the Free Fire API infrastructure
- **Garena Free Fire** for creating the game (unofficial project)
- Community contributors and testers

### 📜 License

```
This project is for educational and informational purposes only.
Please respect Garena's Terms of Service when using this API.
```

---

## ⚠️ Disclaimer

> 🔒 **Important Notice:**
> - This is an **unofficial API** and is not affiliated with, endorsed by, or connected to Garena International or Free Fire.
> - Use this API responsibly and in compliance with Free Fire's [Terms of Service](https://ff.garena.com/terms).
> - The API may experience downtime, changes, or discontinuation without notice.
> - Do not use this API for malicious purposes, account manipulation, or spamming.
> - Player data is fetched from public sources; respect user privacy.

---

## 🤝 Contributing

Found a bug or have a feature request?

1. Check the [LK-TEAM GitHub repositories](https://github.com/PRINCE-LKTEAM) [[6]]
2. Open an issue with detailed information
3. Submit a pull request if you've fixed something

---

## 📞 Support & Contact

| Platform | Handle/Link |
|----------|------------|
| **Telegram** | `@lkteammm` |
| **GitHub** | [PRINCE-LKTEAM](https://github.com/PRINCE-LKTEAM) [[6]] |
| **API Docs** | [freefireinfo-zy9l.onrender.com](https://freefireinfo-zy9l.onrender.com/) |

---

```
⭐ If you find this API useful, please star the original repositories and support LK-TEAM! ⭐
```

---

> 📝 *README generated for https://freefireinfo-zy9l.onrender.com/*  
> 🔄 *Last Updated: $(date)*  
> 💙 *Credits: LK-TEAM*
