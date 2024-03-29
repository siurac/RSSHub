---
pageClass: routes
---

# ACG

## Bangumi Moe

### Latest

<RouteEn author="nczitzk" example="/bangumi" path="/bangumi"/>

### Tags

<RouteEn author="nczitzk" example="/bangumi/chs/1080p" path="/bangumi/:tags?" :paramsDesc="['Tags, empty by default, multiple tags separated by `/`']">

For more tags, please go to [Search torrent](https://bangumi.moe/search/index)

</RouteEn>

## Hanime.tv

### Recently updated

<RouteEn author="EsuRt" example="/hanime/video" path="/hanime/video"/>

## iwara

### User

<RouteEn author="Fatpandac" example="/iwara/users/kelpie/video" path="/iwara/users/:username/:type?" :paramsDesc="['username, can find in userpage', 'video by default']" radar="1" rssbud="1">

| type | video | image |
| :--: | :---: | :---: |
|      | video | image |

</RouteEn>

## Kemono

### Posts

<RouteEn author="nczitzk" example="/kemono" path="/kemono/:source?/:id?" :paramsDesc="['Source, see below, Posts by default', 'User id, can be found in URL']">

Sources

| Posts | Patreon | Pixiv Fanbox | Gumroad | SubscribeStar | DLsite | Discord | Fantia |
| ----- | ------- | ------------ | ------- | ------------- | ------ | ------- | ------ |
| posts | patreon | fanbox       | gumroad | subscribestar | dlsite | discord | fantia |

::: tip Tip

When `posts` is selected as the value of the parameter **source**, the parameter **id** does not take effect.

:::

</RouteEn>

## Touhougarakuta

### Articles

<RouteEn author="ttyfly" path="/touhougarakuta/:language/:type" example="/touhougarakuta/ja/news" :paramsDesc="['language', 'article type']">

Languages:

| Chinese | Japanese | Korean |
| ---- | ---- | ---- |
|  cn  |  ja  |  ko  |

Article types:

|  Index   | Series | Interviews | Novels | Comics | News |
| -------- | ------ | ---------- | ------ | ------ | ---- |
|  index   | series | interviews | novels | comics | news |

| Music review | Game review | Book review  | Where are you |
| ------------ | ----------- | ------------ | ------------- |
| music_review | game_review | book_review  | where_are_you |

**Note:** The index type includes all types of articles. Think twice before using it.

</RouteEn>

## Vol.moe

### vol

<RouteEn author="CoderTonyChan" example="/vol/finish" path="/vol/:mode?" :paramsDesc="['mode type']">

| Comics are serialized | Comics is finshed |
| --------------------- | ----------------- |
| serial                | finish            |

</RouteEn>

## Webtoons

### Comic updates

<RouteEn author="machsix" path="/webtoons/:lang/:category/:name/:id" example="/webtoons/zh-hant/drama/gongzhuweimian/894" :paramsDesc="['Language','Category','Name','ID']"/>

For example: <https://www.webtoons.com/zh-hant/drama/gongzhuweimian/list?title_no=894>, `lang=zh-hant`,`category=drama`,`name=gongzhucheyeweimian`,`id=894`.

### [Naver](https://comic.naver.com)

<RouteEn author="zfanta" example="/webtoons/naver/651673" path="/webtoons/naver/:titleId" :paramsDesc="['titleId of naver webtoon']" />

## 俺の3Dエロ動画(oreno3d)

::: tip Tip

You can use some RSS parsing libraries (like `feedpraser` in `Python`) to receive the video update messages and download them automatically

:::

### Keyword Search

<RouteEn author="xueli-sherryli" example="/oreno3d/search/bronya/latest" path="/oreno3d/search/:keyword/:sort?" :paramsDesc="['Search keyword', 'Sort method, see the table below, `latest` by default']" radar="1" rssbud="1">

| favorites |  hot   | latest | popularity |
| --------- | ------ | ------ | ---------- |
| favorites |  hot   | latest | popularity |

</RouteEn>

### Character Search

<RouteEn author="xueli-sherryli" example="/oreno3d/characters/283/latest" path="/oreno3d/characters/:characterid/:sort?" :paramsDesc="['Character id, can be found in URL' , 'Sort method, see the table above, `latest` by default']" radar="1" rssbud="1"/>

### Author Search

<RouteEn author="xueli-sherryli" example="/oreno3d/authors/3189/latest" path="/oreno3d/authors/:authorid/:sort?" :paramsDesc="['Author id, can be found in URL' , 'Sort method, see the table above, `latest` by default']" radar="1" rssbud="1"/>

### Tags Search

<RouteEn tag="xueli-sherryli" example="/oreno3d/tags/177/latest" path="/oreno3d/tags/:tagid/:sort?" :paramsDesc="['Tag id, can be found in URL', 'Sort method, see the table above, `latest` by default']" radar="1" rssbud="1"/>

### Origins Search

<RouteEn origin="xueli-sherryli" example="/oreno3d/origins/3/latest" path="/oreno3d/origins/:originid/:sort?" :paramsDesc="['Origin id, can be found in URL' , 'Sort method, see the table above, `latest` by default']" radar="1" rssbud="1"/>
