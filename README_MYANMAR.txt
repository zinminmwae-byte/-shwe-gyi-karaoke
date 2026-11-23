# ရွှေကျီး ခေါင်ရည်ဆိုင် Karaoke — ဖုန်းတစ်လုံးတည်းနဲ့ APK ထုတ်ရန်

ဒီ ZIP ထဲမှာ Android app source နဲ့ GitHub Actions cloud-build workflow ပါပါတယ်။ APK ကို ဒီနေရာကနေ ကြိုတင် compile/test မလုပ်ရသေးပါ။ GitHub က cloud computer ပေါ်မှာ build လုပ်ပြီး APK artifact ထုတ်ပေးပါမယ်။

## ဖုန်းကနေ လုပ်ရမယ့်အဆင့်များ

1. ZIP ကို ဖုန်းထဲ Download လုပ်ပြီး Files app နဲ့ Extract လုပ်ပါ။
2. Chrome မှာ https://github.com ကိုဖွင့်ပြီး အခမဲ့ account ဝင်/ဖွင့်ပါ။
3. `+` → `New repository` ကိုနှိပ်ပါ။ Repository name ကို `ShweGyiKaraoke` ထားပြီး `Public` သို့မဟုတ် `Private` ရွေးကာ Create လုပ်ပါ။
4. Repository ထဲက `Add file` → `Upload files` ကိုနှိပ်ပါ။ ZIP ကို မတင်ပါနှင့်။ Extract လုပ်ထားတဲ့ folder အတွင်းက ဖိုင်/ဖိုလ်ဒါအားလုံးကို တင်ပါ။ `.github` folder ကိုလည်း မကျန်စေပါနှင့်။ `Commit changes` ကိုနှိပ်ပါ။
5. Repository ရဲ့ `Actions` tab ကိုဖွင့်ပါ။ `Build ShweGyi Karaoke APK` ကိုရွေးပြီး `Run workflow` ကိုနှိပ်ပါ။ (ပထမဆုံး push တင်ပြီးနောက် အလိုအလျောက်လည်း စတင်နိုင်ပါတယ်။)
6. Build အောင်မြင်လျှင် အဲဒီ run ထဲက `Artifacts` အောက်မှာ `ShweGyi-Karaoke-APK` ကိုနှိပ်ပြီး ZIP artifact ကို download လုပ်ပါ။
7. Download လုပ်ထားတဲ့ artifact ZIP ကို Extract လုပ်ပါ။ `app-debug.apk` ကိုနှိပ်ပြီး Install လုပ်ပါ။ Android က “Install unknown apps” ခွင့်တောင်းလျှင် Chrome/Files အတွက် ခွင့်ပြုပါ။

## App လုပ်ဆောင်ချက်များ / ကန့်သတ်ချက်များ
- ဖုန်းထဲမှ audio ဖိုင်ရွေးဖွင့်နိုင်သည်။
- YouTube ရှာဖွေမှုနှင့် link ဖွင့်မှုကို YouTube app/browser သို့ လွှဲပေးသည်။
- LRC စာသားကို ကိုယ်တိုင်ထည့်လျှင် သီချင်းအချိန်နှင့်လိုက်ပြသည်။
- မိုက်ခရိုဖုန်းခွင့်ပြုချက်နှင့် အသံသွင်းခြင်း ပါဝင်သည်။
- မြန်မာ TTS အသံရရှိမှုသည် ဖုန်းထဲတွင် မြန်မာ voice ရှိ/မရှိပေါ်မူတည်သည်။
- 6.35mm မိုက်ကို ဖုန်းသို့ချိတ်ရန် သင့်တော်သော USB-C OTG audio interface လိုနိုင်သည်။
- YouTube သီချင်းဖွင့်ရန် အင်တာနက်လိုသည်။ သီချင်းဖိုင်များနှင့် စာသားများကို မူပိုင်ခွင့်ခွင့်ပြုထားသည့် ကိုယ်ပိုင်ဖိုင်များမှ ထည့်သုံးပါ။

**မှတ်ချက်:** ဒီနည်းမှာ GitHub account နဲ့ ဖုန်း browser ကနေ ဖိုင်တင်ခြင်းအဆင့်တွေ လိုပါတယ်။ Build မအောင်မြင်လျှင် Actions run ထဲက error ကို screenshot ပို့ပါ။
