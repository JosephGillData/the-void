# 🧭 WEEK 1–2 PLAN: Data Centre Fundamentals

## 🎯 Core Objective

By the end of 2 weeks, you should be able to confidently answer:

> “If I had to build a data centre, what would physically limit me first—and why?”

---

# 🗓️ WEEK 1 — Power + Cooling (The Hard Constraints)

These are the _real bottlenecks_ in AI infrastructure.

---

## 🔌 Day 1–2: Power & Redundancy

![https://images.openai.com/static-rsc-4/c3cwzDVnFiVuNiCGwrKMXL6nc4u4Lh_3F8SDMdZjoDtlzming-SO9RSaklELbIKCq0NuLsiTahPUez6s5FkeuFG1T0H-uwiVWV-uJM0C_9W-gEp4MWQdOp38atC-QFTfltps0vqFUNfhQJjlntgGV1JX6Syb7o38whD0Bl2UToG2T7E_t7hZ1rAofr3lj5Yf?purpose=fullsize](https://images.openai.com/static-rsc-4/iO4oaP__KjLWfxbOmcdTBK7OPn1rpBEzLvN_bq8G3nx-dtiOOZSkSbHx1xiDct9gblhUfZVenKP8fwNpJlJ_wpFmY1jhXszvQXAf4oK-nQePhv3j0J_6kREeJ-XT7FGUgpuI0fuPFMnga4eh8iBJpDxP0aFJyOBEgVWE9F-N414?purpose=inline)

![https://images.openai.com/static-rsc-4/ITe5P7Tn_YSgcJ5jgxkMz_bPK9yRJVeHaRbC6OHbdKpYKX0APwbEYts7RylbyVO5g4uYxDmxXSBRBvjkDtCRiE9ai9DOQ_oiwOQb4ljv8Jrj8mjGJ7PYxQJ3yz5DEbcinA6c6MwcilFdxRQV5HVvdDPx0yPQKfFF04PAft3rq6OsnVV_OpeP6NAH4Z-Pg-cS?purpose=fullsize](https://images.openai.com/static-rsc-4/I41sHg42rWYt8alWUNbjnHP1_WjyIFk7tz42zcrvgv0VhFlz26bssGymOoDPCj-aHI_J_BoxfOpMCCoeRoCcbF1i9SOb2p86VTaFFYLylZ4c734ZrHgCYDo1DYLnaGTqCtapKMabfJ6AXudj3APVARUAF5Dtvh-WHoFc7fUK44k?purpose=inline)

![https://images.openai.com/static-rsc-4/gBla9vgv0CmyfsMSy3TFZKmAhHjDzXPTmNOB2NncMzmKOAUcehafW8HcbhEsSbJrJUbz1U0ADfQYDpgEEpnPGW3YyGNlqbFCrlyXEayHDqzg4WZokzBoVuxJquc_xa6-Y9YOwkXEU3ct1By_hZHJG3kxZc9mViVMN_t3o5HQJe-fmmNjHloTrF3zDkg9au7z?purpose=fullsize](https://images.openai.com/static-rsc-4/3OBhwZa6A5YP3OC62YKRIefCMZUw9GPmHIFfsoWAmuaBKRWxirTGToQD4Ew5MYGfV36YMb4UWJOdcyPtvJoGY_dD42J5MzRrzY6m_K5ucu7RVHbFOeli2CSxNpwpZ2jzTXM_EjZowcxo6nbIUgrdmFodmPwYiUNb3Hg-98yKoqiShlwYjWTaA5f-R31eiOUF?purpose=inline)

6

### What to understand:

- Grid power → UPS → PDU → servers
- What a **UPS (Uninterruptible Power Supply)** actually does
- Why generators exist (and how long they last)
- Redundancy models:
    - N (basic)
    - N+1 (one backup)
    - 2N (fully duplicated)

### Mental model:

Power is _continuous survival_. If it drops → everything dies instantly.

### Your task:

- Draw a simple diagram:  
    `Grid → UPS → Generator → Rack`
- Answer in your own words:
    - “What happens in the first 10 seconds of a power cut?”

---

## ❄️ Day 3–4: Cooling Systems

![https://images.openai.com/static-rsc-4/iaNu6RplASdCCVw9K171R6AEXh9PVfJd21yNRYHJbo_fNjRRbgnavZQbvTWI2FNjwshTWhS1MALXdCRTtObc23M78nbtRJaJ4Yjy0x6HOELDdG_5oBMXnFipyX2aZaroZ5pacc2oPSAjAmeFEypRVllgynad484bUT0nCqptWhaUxafyJJF322PLuXkRetg6?purpose=fullsize](https://images.openai.com/static-rsc-4/jakH0wkayVRR2Suf9O5YLRvJsmSAlzMQTOETGM2Y16Ejb0G8iGVu8yZBZ03I0IyScOjje1pKA2L9WDtoqLPkM036Itt_22dyTQRjB6hq2Iql3YY0XUg1OwGTbZ2EJabNpuPGy_eyx3LM-0kGeFOIXoOCMWtGd4mYCFFNQWVtQVI?purpose=inline)

![https://images.openai.com/static-rsc-4/VAa2qLO8i5G6B5XUs4dJ5pKuVzefo49Uvw4Gk9jZ2LctjXkLaB6dbRq942bbJRjPm8d7Ip6zV5vaAlIXfUdxLfR_l5Q1kOSxmsDif1dWDa5FIAWKmTnxb3SfoAJqrjWI3Pvxdm1JxRzF3b_xTY9bXkWK1tW0uO4XyhC0WT-Oi7we4fXZMXEBCSPciK4qMglR?purpose=fullsize](https://images.openai.com/static-rsc-4/l2JsImfkDq14ARG3aXETVcwOdyQrA_VZyslJJNXnkQ0WMatY6ARPHBGBLiIY9n15Sgq6Xc4sikaMi5dly5MpIyBOcISbSCoNfG82jYffawY2Tm4RW1k33ak2TaXLeAag3mZQ7jwN8N9336hrnu9qJVY-X28xNqVfszLBZ-CPtTQ?purpose=inline)

![https://images.openai.com/static-rsc-4/f1kPE7eF9TDJaiW2IYTXB93kaVB1f9aOf2RW5G0ZQyM8Z1LfOOK3GbYgtbxIaWM_5mtGnIhN2HRAfubKOvQp6DmLOJwtYrCkC7y87GQlwDTefKyULAqE4peQV0yS6h5XX5nnxdrLh4_cghIDZQDsmRq97A6s6qthCFZfofzyZS0CP11K6qicdz8oSgNladqv?purpose=fullsize](https://images.openai.com/static-rsc-4/SlrU6G8JFTWRYpz-opBYexjcl7NAKwszBlw7PHkKDjwe0Da6tcHpuBJxU1BuEdJ702XAxItuG51N6I4nQmK4M9AutUJ_EhgE0kId461bJUFVHnYal_5NM_MonfPtEt1_WJfEhkncru9X8XBL43guk2qfzQ1K45VsQToKuTYJn4M?purpose=inline)

6

### What to understand:

- Servers don’t “use” energy—they turn it into **heat**
- GPUs = extreme heat density
- Cooling types:
    - Air cooling (standard)
    - Liquid cooling (AI-heavy workloads)

### Key insight:

> Cooling—not compute—is often the scaling limit for AI.

### Your task:

- Explain:
    - “Why can’t we just keep adding GPUs indefinitely?”
- Compare:
    - Air vs liquid cooling (1–2 pros/cons each)

---

## 🔁 Day 5: Synthesis (Power + Cooling)

Bring it together:

- Why more compute = more power = more heat
- Why data centres cluster near:
    - Cheap energy
    - Cold climates

### Mini-output:

Write 5 bullet points:

- “The 5 biggest physical constraints in a data centre”

---

## 🧠 Day 6–7: Light Review + Reflection

No new material. Just:

- Re-explain everything _without notes_
- Refine your diagrams

---

# 🗓️ WEEK 2 — Layout + Reliability (Making It Work at Scale)

---

## 🌬️ Day 8–9: Layout & Airflow

![https://images.openai.com/static-rsc-4/sG4yqXR9VIokGfkRRS68XaAfZ0iFT4yNsOYQZZCHLtNcg5yluSIrJrTN0TPMO-Hp6YbJKoXza5m5rynyTCE-Gisvze-fhRYj9Wt5B6jcUopnm-llDpgHs5Q-38U78lsHS19kuht6GVhAoYS5MC8YuQiVfRU4l2EKTx4oeSFVqDfbvVkjAY-UTNfd-COg6KFH?purpose=fullsize](https://images.openai.com/static-rsc-4/uSuXalx8vfkowUHe2ntl2LdM6w56V42TShjJx-BtE57FAAWwG3PoZMM9wzKk796GHIqfIN6MirYH7zjLDuZ_mh5t0tz70vKStTHELMdE6jPsgI3YTNXza4Gb3MNRPZUq567Ulsk-psVvjvVCGzsjXt1uJUl0aYdW-u9RGwjzKcU?purpose=inline)

![https://images.openai.com/static-rsc-4/hmlmQHr5exETaviHrmGfOABjxH88aNcp7hgwquBV4VZ0f_3kkc2DjY5IpXHSImdXQxem_OT5zRz8Q_Q7X8hzvghQX8LJel05sO8-h-n97pdQPJPzLegMb8M3MZ_gvzztRTWXnu2ATqHbqiRRQEXXcQrE11XhSz8c8phgFeT0bve-hIs_NVJbhc8jkW1iHNKz?purpose=fullsize](https://images.openai.com/static-rsc-4/Dbf8kW_KLSSza8B1RbQP5FnycZRmHCinUsaIsw8H_XoYb0incboZ_Jk5uxv5yYwQpmR2kaQ-qWNusNEkgmlWtEoJm02cD_Bx1LSmqz34P7ah_UsLfT3aaaBNZkQ-B6VVONcTkQlTM0C2M3pjtO_NrqncELKVeK5NaoAQLLEmuWo?purpose=inline)

![https://images.openai.com/static-rsc-4/kE8SmuW1lSf6BkzkwkzJu7P7bjxuoWtBHlRfCf-oIgNOR1XkNZZdv3dPwDniYb8ma9gIkLLqXN9G6OrtCG3fxrbedv5sT8s_1KwPbZdeqX9ogd9dxaFmc8Mqq1QC3ncs8z7hC-bPGHM4nWFtI6E5kw8ecSBtJY6LxXDaUcspfYMpxAwSBHfnq2b6CzVXmes-?purpose=fullsize](https://images.openai.com/static-rsc-4/_78D8fP91tGqMnkfp19mV31B8OEh3psXaCJ3NczkON0u0E56Ezr9oP36Rl98C-FO0nEwjRFt4RVDu24rlkuW_bGc687zBo9KzUWMVmTWtZTWMEqO2OAgULdVi8qxfHJO-fm6TF5ecY3_1-L2-lwMQarh2lzMKwTf9JiyBoAYvxo?purpose=inline)

6

### What to understand:

- Hot aisle / cold aisle separation
- Why mixing air = inefficiency
- Rack density (kW per rack)

### Mental model:

You’re managing _air like a fluid system_

### Your task:

- Sketch:
    - Hot aisle vs cold aisle
- Answer:
    - “What goes wrong if airflow is poorly managed?”

---

## 🏢 Day 10–11: Uptime Tiers (Tier I–IV)

![https://images.openai.com/static-rsc-4/1k7a85wdkZgOPIDn8hxudXFjsZAdjbgg0qxp3w8X9cwPnmC1mtuMOFM94PMOEIzf0y7Wd97fRuVevB7GXi05LWl_v6UlopjqbTqgSaz5C2M4bJF0GidkJ8E0mqtnyP6LN7gF-H5xSPUZxDNofqlGkJ3aBP4FiVNtxg8XjUkhzU2RXXeiGDzZ94BrymsR0BKy?purpose=fullsize](https://images.openai.com/static-rsc-4/HJEaI6XEu7gSdD-7_bEo5nVGMvZ5uszjQsnpQETQRKSNnfmhtuvP2GdmhQWTe8Cki8UnYMdnemuYQJq7Fmo_p2lzNADuJ_JgwUh9f4kCTU7v91guEnMiCFnUbLr6EaJH9gg7XKz-KZVvxR_iPScXTd53LLaflv9d-rd9mAT-6JM?purpose=inline)

![https://images.openai.com/static-rsc-4/a-k14xdb63jWJHvCykMl5kpA-Mm2eCFbzI5x0qOh2RGUsQ-G4OUPJQDBacU_e_8txqM1ACKuVuZTOxc_GChOcVf0R0Pt0A65C7yoRZIiDGYPfDqJ5H6s3KNc-TRD8U-s-dd6yRiNBZWqCDgRbRNq4rnMBqWOx99ZKuxp7gCKLQJaDOPxL0fxnf2Bb2ozyeAR?purpose=fullsize](https://images.openai.com/static-rsc-4/5n8jz8HEDuN9f3_UjiUm7aHn-A1wwf5YKUgEbrrex1dl9lFbRE22Md52NFSemcG0vSnmXFB3hIicH94md1tEhHnE8oHzV4hgTNVj4f7etaKHhXCQ9jCov7H8mpzeJCb0CJXEtSJhEzX-n8gHcW0oSJV1IptF-XRk6DrcfZXgims?purpose=inline)

![https://images.openai.com/static-rsc-4/qzUMTUzc9RICnAmfTNpZIMqE6ztMcsewBN2EagQEll06m75eh-nSde8W5fehBAIqWhDsADa6MKD2vNfkfpWmI6GH0LssIpv5hlh62lJF5Wk1WXbSAOWSpghaJsVmiSQ7mgoFIGWotgzWu5pU1x3DUT1UDnut1dHeD--59bIo0mIpRaclGc6y9KXcSUCmU-VL?purpose=fullsize](https://images.openai.com/static-rsc-4/0T4patHRwpYTKI3hLHzMym270c_73bUAt2JkVLB-LT_xvc-sQ4X54bL8econWmZhiQkSHYCdlTavLiAAc6ujTO6F7XMpwKGdUu2hphiSbvANsSRPQwxkIRdS0BziVbJIfgAzQj8_Z5our4fskfNad2qXd2ppk9Az9NngpAZ72Cw?purpose=inline)

6

### What to understand:

- Uptime Institute classification
- Differences:
    - Tier I: basic
    - Tier II: some redundancy
    - Tier III: concurrent maintenance
    - Tier IV: fault tolerant

### Key idea:

> Higher tier = more redundancy = exponentially higher cost

### Your task:

- Answer:
    - “Why doesn’t every company just build Tier IV?”

---

## 🔗 Day 12: Synthesis (Whole System Thinking)

Bring everything together:

- Power ↔ Cooling ↔ Layout ↔ Reliability
- Trade-offs:
    - Cost vs uptime
    - Density vs cooling complexity

### Task:

Write:

- “If I had £100M, what kind of data centre would I build and why?”

---

## ✍️ Day 13–14: Final Output (Non-Negotiable)

### Your 1-page note:

**Title:**

> “How a data centre works (explained simply)”

### Structure:

1. What a data centre is (1–2 paragraphs)
2. Power (how it stays alive)
3. Cooling (why heat is the enemy)
4. Layout (how airflow is controlled)
5. Reliability (tiers + redundancy)
6. Final insight:
    - “The real constraint is ______”

---

# 🧠 How to Approach This (Important)

Don’t treat this like studying.

Instead:

- Think like a **builder**
- Constantly ask:
    - “What breaks first?”
    - “What gets expensive fastest?”
    - “What scales badly?”

---

# ⚡ Optional (High-Leverage Add-On)

If you want to stand out:

- Write 1 short LinkedIn-style post:
    - “The biggest misconception about AI infrastructure is…”
- Keep it simple, insight-driven