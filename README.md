# reaction-roles
Bot Discord yang memungkinkan pengguna untuk menetapkan sendiri peran menggunakan reaksi.

# Mempersiapkan
1. Buat aplikasi anda [Klik Disini!](https://discordapp.com/developers/applications/me) dan ambil token nya.

> Jangan lupa untuk memberi izin `Manage Roles` pada bot Anda!

2. Buka [config.json](https://github.com/zyiang1928/reaction-role-tutorial/blob/master/config.json) dan masukkan token bot nya.

3. Buka [structures/reaction-role.json](https://github.com/zyiang1928/reaction-role-tutorial/blob/master/structures/reaction-role.json) dan mengkonfigurasikan pengaturan anda sendiri:
```js
[ 
  { 
    "messageId" : "MESSAGE_ID",
    "channelId" : "TEXT_CHANNEL_ID",
    "isUnique" : true,
    "emojiRoleMap" : { 
      "EMOJI_1" : ["ROLE_1_ID"], 
      "EMOJI_2" : ["ROLE_2_ID"], 
      "EMOJI_3" : ["ROLE_3_ID", "ROLE_4_ID"],
      //... Tambahkan sebanyak mungkin pemetaan peran emoji yang Anda inginkan.
    }
  },
  //... Tambahkan sebanyak mungkin aturan yang Anda inginkan.]
```

> Jika `isUnique` adalah `true`, pengguna dapat memilih hanya satu kelompok peran. Jika `false`, pengguna dapat memilih grup peran sebanyak yang mereka inginkan.

> `EMOJI_N` bisa menjadi emoji unicode atau id emoji untuk emoji khusus (custom).

> Emoji dapat memetakan ke berbagai peran seperti yang terlihat di `EMOJI_3` di atas.

**Bagaimana? Cukup mudah bukan? Jika anda perlu bantuan silahkan gabung ke server ini [Klik Disini!](https://discord.gg/czHfcuP)**
