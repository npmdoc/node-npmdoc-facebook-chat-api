# api documentation for  [facebook-chat-api (v1.3.0)](https://github.com/Schmavery/facebook-chat-api#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-facebook-chat-api.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-facebook-chat-api) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-facebook-chat-api.svg)](https://travis-ci.org/npmdoc/node-npmdoc-facebook-chat-api)
#### Facebook chat API that doesn't rely on XMPP.  Will NOT be deprecated April 30th 2015.

[![NPM](https://nodei.co/npm/facebook-chat-api.png?downloads=true)](https://www.npmjs.com/package/facebook-chat-api)

[![apidoc](https://npmdoc.github.io/node-npmdoc-facebook-chat-api/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-facebook-chat-api_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-facebook-chat-api/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-facebook-chat-api/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-facebook-chat-api/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Avery, David, Maude, Benjamin"
    },
    "bugs": {
        "url": "https://github.com/Schmavery/facebook-chat-api/issues"
    },
    "dependencies": {
        "bluebird": "^2.9.27",
        "cheerio": "^0.19.0",
        "npmlog": "^1.2.0",
        "request": "^2.53.0"
    },
    "description": "Facebook chat API that doesn't rely on XMPP.  Will NOT be deprecated April 30th 2015.",
    "devDependencies": {
        "mocha": "^2.2.5"
    },
    "directories": {},
    "dist": {
        "shasum": "abb2387b6cd28d8cc017e2a019d9afdd04f7ac0e",
        "tarball": "https://registry.npmjs.org/facebook-chat-api/-/facebook-chat-api-1.3.0.tgz"
    },
    "engines": {
        "node": ">=4.x"
    },
    "gitHead": "5a63981ed40d027930ebc14e4444e2563f7d23a2",
    "homepage": "https://github.com/Schmavery/facebook-chat-api#readme",
    "keywords": [
        "facebook",
        "chat",
        "api"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "schmavery",
            "email": "avery.schmavery@gmail.com"
        }
    ],
    "name": "facebook-chat-api",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/Schmavery/facebook-chat-api.git"
    },
    "scripts": {
        "start": "node server.js",
        "test": "mocha"
    },
    "version": "1.3.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module facebook-chat-api](#apidoc.module.facebook-chat-api)
1.  object <span class="apidocSignatureSpan">facebook-chat-api.</span>utils

#### [module facebook-chat-api.utils](#apidoc.module.facebook-chat-api.utils)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>arrToForm (form)](#apidoc.element.facebook-chat-api.utils.arrToForm)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatCookie (arr, url)](#apidoc.element.facebook-chat-api.utils.formatCookie)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatDate (date)](#apidoc.element.facebook-chat-api.utils.formatDate)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatDeltaMessage (m)](#apidoc.element.facebook-chat-api.utils.formatDeltaMessage)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatEvent (m)](#apidoc.element.facebook-chat-api.utils.formatEvent)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatMessage (m)](#apidoc.element.facebook-chat-api.utils.formatMessage)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatPresence (presence, userID)](#apidoc.element.facebook-chat-api.utils.formatPresence)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatRead (event)](#apidoc.element.facebook-chat-api.utils.formatRead)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatReadReceipt (event)](#apidoc.element.facebook-chat-api.utils.formatReadReceipt)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatThread (data)](#apidoc.element.facebook-chat-api.utils.formatThread)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatTyp (event)](#apidoc.element.facebook-chat-api.utils.formatTyp)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>generateAccessiblityCookie ()](#apidoc.element.facebook-chat-api.utils.generateAccessiblityCookie)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>generateOfflineThreadingID ()](#apidoc.element.facebook-chat-api.utils.generateOfflineThreadingID)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>generatePresence (userID)](#apidoc.element.facebook-chat-api.utils.generatePresence)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>generateThreadingID (clientID)](#apidoc.element.facebook-chat-api.utils.generateThreadingID)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>generateTimestampRelative ()](#apidoc.element.facebook-chat-api.utils.generateTimestampRelative)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>get (url, jar, qs)](#apidoc.element.facebook-chat-api.utils.get)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>getAppState (jar)](#apidoc.element.facebook-chat-api.utils.getAppState)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>getFrom (str, startToken, endToken)](#apidoc.element.facebook-chat-api.utils.getFrom)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>getGUID ()](#apidoc.element.facebook-chat-api.utils.getGUID)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>getJar (store)](#apidoc.element.facebook-chat-api.utils.getJar)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>getSignatureID ()](#apidoc.element.facebook-chat-api.utils.getSignatureID)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>getType (obj)](#apidoc.element.facebook-chat-api.utils.getType)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>isReadableStream (obj)](#apidoc.element.facebook-chat-api.utils.isReadableStream)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>makeDefaults (html, userID)](#apidoc.element.facebook-chat-api.utils.makeDefaults)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>makeParsable (html)](#apidoc.element.facebook-chat-api.utils.makeParsable)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>parseAndCheckLogin (jar, defaultFuncs)](#apidoc.element.facebook-chat-api.utils.parseAndCheckLogin)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>post (url, jar, form)](#apidoc.element.facebook-chat-api.utils.post)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>postFormData (url, jar, form, qs)](#apidoc.element.facebook-chat-api.utils.postFormData)
1.  [function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>saveCookies (jar)](#apidoc.element.facebook-chat-api.utils.saveCookies)



# <a name="apidoc.module.facebook-chat-api"></a>[module facebook-chat-api](#apidoc.module.facebook-chat-api)



# <a name="apidoc.module.facebook-chat-api.utils"></a>[module facebook-chat-api.utils](#apidoc.module.facebook-chat-api.utils)

#### <a name="apidoc.element.facebook-chat-api.utils.arrToForm"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>arrToForm (form)](#apidoc.element.facebook-chat-api.utils.arrToForm)
- description and source-code
```javascript
function arrToForm(form) {
  return arrayToObject(form, function(v) {return v.name;}, function(v) {return v.val;});
}
```
- example usage
```shell
...
  arr.push({val: $(v).val(), name: $(v).attr("name")});
});

arr = arr.filter(function(v) {
  return v.val && v.val.length;
});

var form = utils.arrToForm(arr);
form.lsd = utils.getFrom(html, "[\"LSD\",[],{\"token\":\"", "\"}");
form.lgndim = new Buffer("{\"w\":1440,\"h\":900,\"aw\":1440,\"ah\":834,\"c\":24}").toString('base64');
form.email = email;
form.pass = password;
form.default_persistent = '0';
form.lgnrnd = utils.getFrom(html, "name=\"lgnrnd\" value=\"", "\"");
form.locale = 'en_US';
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.formatCookie"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatCookie (arr, url)](#apidoc.element.facebook-chat-api.utils.formatCookie)
- description and source-code
```javascript
function formatCookie(arr, url) {
  return arr[0]+"="+arr[1]+"; Path=" + arr[3] + "; Domain="+url+".com";
}
```
- example usage
```shell
...
// which happen to be conveniently indicated with a _js_ in front of their
// variable name.
//
// ---------- Very Hacky Part Starts -----------------
var willBeCookies = html.split("\"_js_");
willBeCookies.slice(1).map(function(val) {
  var cookieData = JSON.parse("[\"" + utils.getFrom(val, "", "]") + "]");
  jar.setCookie(utils.formatCookie(cookieData, "facebook"), "https://www.facebook.com");
});
// ---------- Very Hacky Part Ends -----------------

log.info("login", "Logging in...");
return utils
  .post("https://www.facebook.com/login.php?login_attempt=1&lwv=110", jar, form)
  .then(utils.saveCookies(jar))
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.formatDate"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatDate (date)](#apidoc.element.facebook-chat-api.utils.formatDate)
- description and source-code
```javascript
function formatDate(date) {
  var d = date.getUTCDate(); d = d >= 10 ? d : '0'+d;
  var h = date.getUTCHours(); h = h >= 10 ? h : '0'+h;
  var m = date.getUTCMinutes(); m = m >= 10 ? m : '0'+m;
  var s = date.getUTCSeconds(); s = s >= 10 ? s : '0'+s;
  return NUM_TO_DAY[date.getUTCDay()] + ', ' +
    d+' '+ NUM_TO_MONTH[date.getUTCMonth()] +' '+ date.getUTCFullYear() +' '+
    h+':'+m+':'+s+' GMT';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.facebook-chat-api.utils.formatDeltaMessage"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatDeltaMessage (m)](#apidoc.element.facebook-chat-api.utils.formatDeltaMessage)
- description and source-code
```javascript
function formatDeltaMessage(m){
  var md = m.delta.messageMetadata;
  return {
    type: "message",
    senderID: md.actorFbId,
    body: m.delta.body,
    threadID: (md.threadKey.threadFbId || md.threadKey.otherUserFbId).toString(),
    messageID: md.messageId,
    attachments: (m.delta.attachments || []).map(v => _formatAttachment(v)),
    timestamp: md.timestamp,
    isGroup: !!md.threadKey.threadFbId
  }
}
```
- example usage
```shell
...
break;
            case 'delta':
if (ctx.globalOptions.pageID || (v.delta.class !== "NewMessage" && !ctx.globalOptions.listenEvents)) return

if (v.delta.class == "NewMessage") {
  (function resolveAttachmentUrl(i) {
    if (i == v.delta.attachments.length) {
      var fmtMsg = utils.formatDeltaMessage(v);
      return (!ctx.globalOptions.selfListen && fmtMsg.senderID === ctx.userID) ? undefined : globalCallback(null, fmtMsg);
    } else {
      if (v.delta.attachments[i].mercury.attach_type == 'photo') {
        defaultFuncs
          .get("https://www.facebook.com/mercury/attachments/photo/?photo_id=" + v.delta.attachments[i].fbid, ctx.jar, {})
          .then(utils.parseAndCheckLogin(ctx.jar, defaultFuncs))
          .then(function (resData) {
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.formatEvent"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatEvent (m)](#apidoc.element.facebook-chat-api.utils.formatEvent)
- description and source-code
```javascript
function formatEvent(m) {
  var logMessageType;
  var logMessageData;

  // log:thread-color => {theme_color}
  // log:user-nickname => {participant_id, nickname}
  // log:thread-icon => {thread_icon}
  // log:thread-name => {name}
  // log:subscribe => {addedParticipants - [Array]}
  // log:unsubscribe => {leftParticipantFbId}

  switch (m.class) {
    case 'AdminTextMessage':
      logMessageData = m.untypedData;
      switch (m.type) {
        case 'change_thread_theme':
          logMessageType = "log:thread-color";
          break;
        case 'change_thread_nickname':
          logMessageType = "log:user-nickname";
          break;
        case 'change_thread_icon':
          logMessageType = "log:thread-icon";
          break;
      }
      break;
    case 'ThreadName':
      logMessageType = "log:thread-name";
      logMessageData = { name: m.name };
      break;
    case 'ParticipantsAddedToGroupThread':
      logMessageType = "log:subscribe";
      logMessageData = { addedParticipants: m.addedParticipants }
      break;
    case 'ParticipantLeftGroupThread':
      logMessageType = "log:unsubscribe";
      logMessageData = { leftParticipantFbId: m.leftParticipantFbId }
      break;
  }

  return {
    type: "event",
    threadID: m.messageMetadata.threadKey.threadFbId || m.messageMetadata.threadKey.otherUserFbId,
    logMessageType: logMessageType,
    logMessageData: logMessageData,
    logMessageBody: m.messageMetadata.adminText,
    author: m.messageMetadata.actorFbId
  };
}
```
- example usage
```shell
...
          break;
        default:
          return;
      }
    case 'ThreadName':
    case 'ParticipantsAddedToGroupThread':
    case 'ParticipantLeftGroupThread':
      var formattedEvent = utils.formatEvent(v.delta);
      return (!ctx.globalOptions.selfListen && formattedEvent.author.toString() === ctx.userID || !ctx.loggedIn)
        ? undefined
        : globalCallback(null, formattedEvent);
  }

  break;
case 'messaging':
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.formatMessage"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatMessage (m)](#apidoc.element.facebook-chat-api.utils.formatMessage)
- description and source-code
```javascript
function formatMessage(m) {
  var originalMessage = m.message ? m.message : m;
  var obj = {
    type: "message",
    senderName: originalMessage.sender_name,
    senderID: originalMessage.sender_fbid.toString(),
    participantNames: (originalMessage.group_thread_info ? originalMessage.group_thread_info.participant_names : [originalMessage
.sender_name.split(' ')[0]]),
    participantIDs: (originalMessage.group_thread_info ? originalMessage.group_thread_info.participant_ids.map(function(v) {return
 v.toString();}) : [originalMessage.sender_fbid]),
    body: originalMessage.body,
    threadID: originalMessage.tid && originalMessage.tid.split(".")[0] === "id" ? originalMessage.tid.split('.')[1] : originalMessage
.thread_fbid || originalMessage.other_user_fbid,
    threadName: (originalMessage.group_thread_info ? originalMessage.group_thread_info.name : originalMessage.sender_name),
    location: originalMessage.coordinates ? originalMessage.coordinates : null,
    messageID: originalMessage.mid ? originalMessage.mid.toString() : originalMessage.message_id,
    attachments: formatAttachment(originalMessage.attachments, originalMessage.attachmentIds, originalMessage.attachment_map, originalMessage
.share_map),
    timestamp: originalMessage.timestamp,
    timestampAbsolute: originalMessage.timestamp_absolute,
    timestampRelative: originalMessage.timestamp_relative,
    timestampDatetime: originalMessage.timestamp_datetime,
    tags: originalMessage.tags
  };

  if(m.type === "pages_messaging") obj.pageID = m.realtime_viewer_fbid.toString();
  obj.isGroup = obj.participantIDs.length > 2;

  return obj;
}
```
- example usage
```shell
...
                                           v.message.sender_fbid.toString() === ctx.globalOptions.pageID)) ||
        v.realtime_viewer_fbid.toString() !== ctx.globalOptions.pageID) {
        return;
      }

      atLeastOne = true;
      if (ctx.loggedIn) {
        return globalCallback(null, utils.formatMessage(v));
      }
      break;
  }
});

if(atLeastOne) {
  // Send deliveryReceipt notification to the server
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.formatPresence"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatPresence (presence, userID)](#apidoc.element.facebook-chat-api.utils.formatPresence)
- description and source-code
```javascript
function formatPresence(presence, userID) {
  return {
    type: "presence",
    timestamp: presence.la * 1000,
    userID: userID,
    statuses: presence.a
  };
}
```
- example usage
```shell
...
  // TODO: what happens when you're logged in as a page?
  if(!ctx.globalOptions.updatePresence) {
    return;
  }

  // There should be only one key inside overlay
  Object.keys(v.overlay).map(function(userID) {
    var formattedPresence = utils.formatPresence(v.overlay[userID], userID);
    if(ctx.loggedIn) {
      return globalCallback(null, formattedPresence);
    }
  });
  break;
case 'delta':
  if (ctx.globalOptions.pageID || (v.delta.class !== "NewMessage" && !ctx.globalOptions.listenEvents)) return
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.formatRead"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatRead (event)](#apidoc.element.facebook-chat-api.utils.formatRead)
- description and source-code
```javascript
function formatRead(event) {
  return {
    threadID: ((event.chat_ids && event.chat_ids[0]) || (event.thread_fbids && event.thread_fbids[0])).toString(),
    time: event.timestamp,
    type: 'read'
  };
}
```
- example usage
```shell
...
  switch (event.event) {
    // "read_receipt" event triggers when other people read the user's messages.
    case 'read_receipt':
      globalCallback(null, utils.formatReadReceipt(event));
      return true;
    // "read event" triggers when the user read other people's messages.
    case 'read':
      globalCallback(null, utils.formatRead(event));
      return true;
    default:
      return false;
  }
}

function listen() {
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.formatReadReceipt"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatReadReceipt (event)](#apidoc.element.facebook-chat-api.utils.formatReadReceipt)
- description and source-code
```javascript
function formatReadReceipt(event) {
  return {
    reader: event.reader.toString(),
    time: event.time,
    threadID: (event.thread_fbid || event.reader).toString(),
    type: 'read_receipt',
  };
}
```
- example usage
```shell
...
 * and returns true if it did handle an event (and called the globalCallback).
 * Returns false otherwise.
 */
function handleMessagingEvents(event) {
  switch (event.event) {
    // "read_receipt" event triggers when other people read the user's messages.
    case 'read_receipt':
      globalCallback(null, utils.formatReadReceipt(event));
      return true;
    // "read event" triggers when the user read other people's messages.
    case 'read':
      globalCallback(null, utils.formatRead(event));
      return true;
    default:
      return false;
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.formatThread"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatThread (data)](#apidoc.element.facebook-chat-api.utils.formatThread)
- description and source-code
```javascript
function formatThread(data) {
  return {
    threadID: data.thread_fbid.toString(),
    participants: data.participants.map(function(v) { return v.replace('fbid:', ''); }),
    participantIDs: data.participants.map(function(v) { return v.replace('fbid:', ''); }),
    formerParticipants: data.former_participants,
    name: data.name,
    nicknames: data.custom_nickname,
    snippet: data.snippet,
    snippetHasAttachment: data.snippet_has_attachment,
    snippetAttachments: data.snippet_attachments,
    snippetSender: (data.snippet_sender || '').replace('fbid:', ''),
    unreadCount: data.unread_count,
    messageCount: data.message_count,
    imageSrc: data.image_src,
    timestamp: data.timestamp,
    serverTimestamp: data.server_timestamp, // what is this?
    muteSettings: data.muteSettings,
    isCanonicalUser: data.is_canonical_user,
    isCanonical: data.is_canonical,
    canonicalFbid: data.canonical_fbid,
    isSubscribed: data.is_subscribed,
    rootMessageThreadingID: data.root_message_threading_id,
    folder: data.folder,
    isArchived: data.is_archived,
    recipientsLoadable: data.recipients_loadable,
    hasEmailParticipant: data.has_email_participant,
    readOnly: data.read_only,
    canReply: data.can_reply,
    composerEnabled: data.composer_enabled,
    blockedParticipants: data.blocked_participants,
    lastMessageID: data.last_message_id
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.facebook-chat-api.utils.formatTyp"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>formatTyp (event)](#apidoc.element.facebook-chat-api.utils.formatTyp)
- description and source-code
```javascript
function formatTyp(event) {
  return {
    isTyping: !!event.st,
    from: event.from.toString(),
    threadID: (event.to || event.thread_fbid || event.from).toString(),
    // When receiving typ indication from mobile, 'from_mobile' isn't set.
    // If it is, we just use that value.
    fromMobile: event.hasOwnProperty('from_mobile') ? event.from_mobile : true,
    userID: (event.realtime_viewer_fbid || event.from).toString(),
    type: 'typ',
  };
}
```
- example usage
```shell
...
case 'ttyp':
case 'typ':
  if(!ctx.globalOptions.listenEvents ||
    (!ctx.globalOptions.selfListen && v.from.toString() === ctx.userID)) {
    return;
  }

  return globalCallback(null, utils.formatTyp(v));
  break;
case 'buddylist_overlay':
  // TODO: what happens when you're logged in as a page?
  if(!ctx.globalOptions.updatePresence) {
    return;
  }
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.generateAccessiblityCookie"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>generateAccessiblityCookie ()](#apidoc.element.facebook-chat-api.utils.generateAccessiblityCookie)
- description and source-code
```javascript
function generateAccessiblityCookie() {
  var time = Date.now();
  return encodeURIComponent(
    JSON.stringify({
      sr: 0,
      'sr-ts': time,
      jk: 0,
      'jk-ts': time,
      kb: 0,
      'kb-ts': time,
      hcm: 0,
      'hcm-ts': time
    }
  ));
}
```
- example usage
```shell
...
  msgs_recv: 0
};
var presence = utils.generatePresence(ctx.userID);
ctx.jar.setCookie("presence=" + presence + "; path=/; domain=.facebook.com; secure", "https://www.facebook.com");
ctx.jar.setCookie("presence=" + presence + "; path=/; domain=.messenger.com; secure", "https://www.messenger.com");
ctx.jar.setCookie("locale=en_US; path=/; domain=.facebook.com; secure", "https://www.facebook.com");
ctx.jar.setCookie("locale=en_US; path=/; domain=.messenger.com; secure", "https://www.messenger.com");
ctx.jar.setCookie("a11y=" + utils.generateAccessiblityCookie() + "; path=/; domain=.facebook.com; secure", "https://www.facebook
.com");

return utils
  .get("https://0-edge-chat.facebook.com/pull", ctx.jar, form)
  .then(utils.saveCookies(ctx.jar))
  .then(function(res) {
    var ret = null;
    try {
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.generateOfflineThreadingID"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>generateOfflineThreadingID ()](#apidoc.element.facebook-chat-api.utils.generateOfflineThreadingID)
- description and source-code
```javascript
function generateOfflineThreadingID() {
  var ret = Date.now();
  var value = Math.floor(Math.random() * 4294967295);
  var str = ("0000000000000000000000" + value.toString(2)).slice(-22);
  var msgs = ret.toString(2) + str;
  return binaryToDecimal(msgs);
}
```
- example usage
```shell
...
  throw {error: "ThreadID should be of type Number or String and not " + utils.getType(threadID) + "."};
}

if (utils.getType(userID) !== "Array") {
  userID = [userID];
}

var messageAndOTID = utils.generateOfflineThreadingID();
var form = {
  'client' : 'mercury',
  'action_type' : 'ma-type:log-message',
  'author' : 'fbid:' + ctx.userID,
  'thread_id' : '',
  'timestamp' : Date.now(),
  'timestamp_absolute' : 'Today',
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.generatePresence"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>generatePresence (userID)](#apidoc.element.facebook-chat-api.utils.generatePresence)
- description and source-code
```javascript
function generatePresence(userID) {
  var time = Date.now();
  return "E" + presenceEncode(JSON.stringify({
    "v": 3,
    "time": parseInt(time / 1000, 10),
    "user": userID,
    "state": {
      "ut": 0,
      "t2": [],
      "lm2": null,
      "uct2": time,
      "tr": null,
      "tw": Math.floor(Math.random() * 4294967295) + 1,
      "at": time
    },
    "ch":{
      ["p_" + userID]: 0
    }
  }))
}
```
- example usage
```shell
...
  viewer_uid : ctx.userID,
  uid : ctx.userID,
  state : 'active',
  idle : 0,
  cap : 8,
  msgs_recv: 0
};
var presence = utils.generatePresence(ctx.userID);
ctx.jar.setCookie("presence=" + presence + "; path=/; domain=.facebook.com; secure", "https://www.facebook.com");
ctx.jar.setCookie("presence=" + presence + "; path=/; domain=.messenger.com; secure", "https://www.messenger.com");
ctx.jar.setCookie("locale=en_US; path=/; domain=.facebook.com; secure", "https://www.facebook.com");
ctx.jar.setCookie("locale=en_US; path=/; domain=.messenger.com; secure", "https://www.messenger.com");
ctx.jar.setCookie("a11y=" + utils.generateAccessiblityCookie() + "; path=/; domain=.facebook.com; secure", "https://www.facebook
.com");

return utils
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.generateThreadingID"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>generateThreadingID (clientID)](#apidoc.element.facebook-chat-api.utils.generateThreadingID)
- description and source-code
```javascript
function generateThreadingID(clientID) {
  var k = Date.now();
  var l = Math.floor(Math.random() * 4294967295);
  var m = clientID;
  return ("<" + k + ":" + l + "-" + m + "@mail.projektitan.com>");
}
```
- example usage
```shell
...
  'is_spoof_warning' : false,
  'source' : 'source:chat:web',
  'source_tags[0]' : 'source:chat',
  'log_message_type' : 'log:subscribe',
  'status' : '0',
  'offline_threading_id' : messageAndOTID,
  'message_id' : messageAndOTID,
  'threading_id': utils.generateThreadingID(ctx.clientID),
  'manual_retry_cnt' : '0',
  'thread_fbid' : threadID,
};

for (var i = 0; i < userID.length; i++){
  if (utils.getType(userID[i]) !== "Number" && utils.getType(userID[i]) !== "String") {
    throw {error: "Elements of userID should be of type Number or String and not " + utils.getType(userID[i]) + "."};
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.generateTimestampRelative"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>generateTimestampRelative ()](#apidoc.element.facebook-chat-api.utils.generateTimestampRelative)
- description and source-code
```javascript
function generateTimestampRelative() {
  var d = new Date();
  return d.getHours() + ":" + padZeros(d.getMinutes());
}
```
- example usage
```shell
...
    var form = {
'client' : 'mercury',
'action_type' : 'ma-type:log-message',
'author' : 'fbid:' + ctx.userID,
'thread_id' : '',
'timestamp' : Date.now(),
'timestamp_absolute' : 'Today',
'timestamp_relative' : utils.generateTimestampRelative(),
'timestamp_time_passed' : '0',
'is_unread' : false,
'is_cleared' : false,
'is_forward' : false,
'is_filtered_content' : false,
'is_filtered_content_bh':false,
'is_filtered_content_account':false,
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.get"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>get (url, jar, qs)](#apidoc.element.facebook-chat-api.utils.get)
- description and source-code
```javascript
function get(url, jar, qs) {
  // I'm still confused about this
  if(getType(qs) === "Object") {
    for(var prop in qs) {
      if(qs.hasOwnProperty(prop) && getType(qs[prop]) === "Object") {
        qs[prop] = JSON.stringify(qs[prop]);
      }
    }
  }
  var op = {
    headers: getHeaders(url),
    timeout: 60000,
    qs: qs,
    url: url,
    method: "GET",
    jar: jar,
    gzip: true
  };

  return request(op).then(function(res) {return res[0];});
}
```
- example usage
```shell
...
        }

        // This means the account has login approvals turned on.
        if (headers.location.indexOf('https://www.facebook.com/checkpoint/') > -1) {
var nextURL = 'https://www.facebook.com/checkpoint/?next=https%3A%2F%2Fwww.facebook.com%2Fhome.php';

return utils
  .get(headers.location, jar)
  .then(utils.saveCookies(jar))
  .then(function(res) {
    var html = res.body;
    // Make the form in advance which will contain the fb_dtsg and nh
    var $ = cheerio.load(html);
    var arr = [];
    $("form input").map(function(i, v){
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.getAppState"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>getAppState (jar)](#apidoc.element.facebook-chat-api.utils.getAppState)
- description and source-code
```javascript
function getAppState(jar){
  return jar
    .getCookies("https://www.facebook.com")
    .concat(jar.getCookies("https://facebook.com"))
    .concat(jar.getCookies("https://www.messenger.com"));
}
```
- example usage
```shell
...
2. Why doesn't 'sendMessage' always work when I'm logged in as a page?
> Pages can't start conversations with users directly; this is to prevent pages from spamming users.

3. What do I do when 'login' doesn't work?
> First check that you can login to Facebook using the website. If login approvals are enabled, you might be logging in incorrectly
. For how to handle login approvals, read our docs on ['login'](DOCS.md#login).

4. How can I avoid logging in every time?  Can I log into a previous session?
> We support caching everything relevant for you to bypass login. 'api.getAppState()' returns an object that you can save and pass
 into login as '{appState: mySavedAppState}' instead of the credentials object.  If this fails, your session has expired.

5. Do you support sending messages as a page?
> Yes, set the pageID option on login (this doesn't work if you set it using api.setOptions, it affects the login process).
> '''js
> login(credentials, {pageID: xxxxx}, function(api) { ... }
> '''
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.getFrom"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>getFrom (str, startToken, endToken)](#apidoc.element.facebook-chat-api.utils.getFrom)
- description and source-code
```javascript
function getFrom(str, startToken, endToken) {
  var start = str.indexOf(startToken) + startToken.length;
  if(start < startToken.length) return "";

  var lastHalf = str.substring(start);
  var end = lastHalf.indexOf(endToken);
  if (end === -1) {
    throw Error("Could not find endTime '" + endToken + "' in the given string.");
  }
  return lastHalf.substring(0, end);
}
```
- example usage
```shell
...
});

arr = arr.filter(function(v) {
  return v.val && v.val.length;
});

var form = utils.arrToForm(arr);
form.lsd = utils.getFrom(html, "[\"LSD\",[],{\"token\":\"", "\"}");
form.lgndim = new Buffer("{\"w\":1440,\"h\":900,\"aw\":1440,\"ah\":834,\"c\":24}").toString('base64');
form.email = email;
form.pass = password;
form.default_persistent = '0';
form.lgnrnd = utils.getFrom(html, "name=\"lgnrnd\" value=\"", "\"");
form.locale = 'en_US';
form.timezone = '240';
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.getGUID"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>getGUID ()](#apidoc.element.facebook-chat-api.utils.getGUID)
- description and source-code
```javascript
function getGUID() {
<span class="apidocCodeCommentSpan">  /** @type {number} */
</span>  var sectionLength = Date.now();
  /** @type {string} */
  var id = "xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx".replace(/[xy]/g, function(c) {
    /** @type {number} */
    var r = Math.floor((sectionLength + Math.random() * 16) % 16);
    /** @type {number} */
    sectionLength = Math.floor(sectionLength / 16);
    /** @type {string} */
    var _guid = (c == "x" ? r : r & 7 | 8).toString(16);
    return _guid;
  });
  return id;
}
```
- example usage
```shell
...

var form = {
  'value' : name.toLowerCase(),
  'viewer' : ctx.userID,
  'rsp' : "search",
  'context' : "search",
  'path' : "/home.php",
  'request_id' : utils.getGUID(),
};

defaultFuncs
  .get("https://www.facebook.com/ajax/typeahead/search.php", ctx.jar, form)
  .then(utils.parseAndCheckLogin(ctx.jar, defaultFuncs))
  .then(function(resData) {
    if (resData.error) {
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.getJar"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>getJar (store)](#apidoc.element.facebook-chat-api.utils.getJar)
- description and source-code
```javascript
getJar = function (store) {
  return cookies.jar(store)
}
```
- example usage
```shell
...
    });
};
}

// Helps the login
function loginHelper(appState, email, password, globalOptions, callback) {
var mainPromise = null;
var jar = utils.getJar();

// If we're given an appState we loop through it and save each cookie
// back into the jar.
if(appState) {
  appState.map(function(c) {
    var str = c.key + "=" + c.value + "; expires=" + c.expires + "; domain=" + c.domain + "; path=" + c.path + ";";
    jar.setCookie(str, "http://" + c.domain);
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.getSignatureID"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>getSignatureID ()](#apidoc.element.facebook-chat-api.utils.getSignatureID)
- description and source-code
```javascript
function getSignatureID(){
  return Math.floor(Math.random() * 2147483648).toString(16);
}
```
- example usage
```shell
...
    'status' : '0',
    'offline_threading_id' : messageAndOTID,
    'message_id' : messageAndOTID,
    'threading_id': utils.generateThreadingID(ctx.clientID),
    'ephemeral_ttl_mode:': '0',
    'manual_retry_cnt' : '0',
    'has_attachment' : !!(msg.attachment || msg.url || msg.sticker),
    'signatureID' : utils.getSignatureID(),
  };

  handleSticker(msg, form, callback,
    () => handleAttachment(msg, form, callback,
      () => handleUrl(msg, form, callback,
        () => send(form, threadID, messageAndOTID, callback))));
};
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.getType"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>getType (obj)](#apidoc.element.facebook-chat-api.utils.getType)
- description and source-code
```javascript
function getType(obj) {
  return Object.prototype.toString.call(obj).slice(8, -1);
}
```
- example usage
```shell
...
  .catch(function(e) {
    log.error("login", e.error || e);
    callback(e);
  });
}

function login(loginData, options, callback) {
if(utils.getType(options) === 'Function') {
  callback = options;
  options = {};
}

var globalOptions = {
  selfListen: false,
  listenEvents: false,
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.isReadableStream"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>isReadableStream (obj)](#apidoc.element.facebook-chat-api.utils.isReadableStream)
- description and source-code
```javascript
function isReadableStream(obj) {
  return obj instanceof stream.Stream &&
    getType(obj._read) === 'Function' &&
    getType(obj._readableState) === 'Object';
}
```
- example usage
```shell
...

module.exports = function(defaultFuncs, api, ctx) {
  function uploadAttachment(attachments, callback) {
    var uploads = [];

    // create an array of promises
    for (var i = 0; i < attachments.length; i++) {
if (!utils.isReadableStream(attachments[i])) {
  throw {error: "Attachment should be a readable stream and not " + utils.getType(attachments[i]) + "."};
}

var form = {
  upload_1024: attachments[i],
  'voice_clip': 'true',
};
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.makeDefaults"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>makeDefaults (html, userID)](#apidoc.element.facebook-chat-api.utils.makeDefaults)
- description and source-code
```javascript
function makeDefaults(html, userID) {
  var reqCounter = 1;
  var fb_dtsg = getFrom(html, "name=\"fb_dtsg\" value=\"", "\"");
  var ttstamp = "";
  for (var i = 0; i < fb_dtsg.length; i++) {
    ttstamp += fb_dtsg.charCodeAt(i);
  }
  ttstamp += '2';
  var revision = getFrom(html, "revision\":",",");

  function mergeWithDefaults(obj) {
    var newObj = {
      __user: userID,
      __req: (reqCounter++).toString(36),
      __rev: revision,
      __a: 1,
      fb_dtsg: fb_dtsg,
      ttstamp: ttstamp,
    };

    if(!obj) return newObj;

    for(var prop in obj) {
      if(obj.hasOwnProperty(prop)) {
        if (!newObj[prop]) {
          newObj[prop] = obj[prop];
        }
      }
    }

    return newObj;
  }

  function postWithDefaults(url, jar, form) {
    return post(url, jar, mergeWithDefaults(form));
  }

  function getWithDefaults(url, jar, qs) {
    return get(url, jar, mergeWithDefaults(qs));
  }

  function postFormDataWithDefault(url, jar, form, qs) {
    return postFormData(url, jar, mergeWithDefaults(form), mergeWithDefaults(qs));
  }

  return {
    get: getWithDefaults,
    post: postWithDefaults,
    postFormData: postFormDataWithDefault,
  };
}
```
- example usage
```shell
...
  'removeUserFromGroup',
  'searchForThread',
  'sendMessage',
  'sendTypingIndicator',
  'setTitle',
];

var defaultFuncs = utils.makeDefaults(html, userID);

// Load all api functions in a loop
apiFuncNames.map(function(v) {
  api[v] = require('./src/' + v)(defaultFuncs, api, ctx);
});

return [ctx, defaultFuncs, api];
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.makeParsable"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>makeParsable (html)](#apidoc.element.facebook-chat-api.utils.makeParsable)
- description and source-code
```javascript
function makeParsable(html) {
  return html.replace(/for\s*\(\s*;\s*;\s*\)\s*;\s*/, "");
}
```
- example usage
```shell
...

  return utils
    .get("https://0-edge-chat.facebook.com/pull", ctx.jar, form)
    .then(utils.saveCookies(ctx.jar))
    .then(function(res) {
      var ret = null;
      try {
        ret = JSON.parse(utils.makeParsable(res.body));
      } catch(e) {
        throw {error: "Error inside first pull request. Received HTML instead of JSON. Logging in inside a browser might help fix
 this."};
      }

      return ret;
    });
})
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.parseAndCheckLogin"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>parseAndCheckLogin (jar, defaultFuncs)](#apidoc.element.facebook-chat-api.utils.parseAndCheckLogin)
- description and source-code
```javascript
function parseAndCheckLogin(jar, defaultFuncs) {
  return function(data) {
    return bluebird.try(function() {
      log.verbose("parseAndCheckLogin", data.body);
      if (data.statusCode >= 500 && data.statusCode < 600) {
        log.warn("parseAndCheckLogin", "Got status code " + data.statusCode + " retrying...");
        var url = data.request.uri.protocol + "//" + data.request.uri.hostname + data.request.uri.pathname;
        if (data.request.headers['Content-Type'].split(";")[0] === "multipart/form-data") {
          return defaultFuncs
            .postFormData(url, jar, data.request.formData, {})
            .then(parseAndCheckLogin(jar));
        } else {
          return defaultFuncs
            .post(url, jar, data.request.formData)
            .then(parseAndCheckLogin(jar));
        }
      }
      if (data.statusCode !== 200) throw new Error("parseAndCheckLogin got status code: " + data.statusCode + ". Bailing out of
trying to parse response.");

      var res = null;
      try {
        res = JSON.parse(makeParsable(data.body));
      } catch(e) {
        throw {
          error: "JSON.parse error. Check the 'detail' property on this error.",
          detail: e,
          res: data.body
        };
      }

      // TODO: handle multiple cookies?
      if (res.jsmods
          && res.jsmods.require
          && Array.isArray(res.jsmods.require[0])
          && res.jsmods.require[0][0] === "Cookie") {
        res.jsmods.require[0][3][0] = res.jsmods.require[0][3][0].replace("_js_", "");
        var cookie = formatCookie(res.jsmods.require[0][3], "facebook");
        var cookie2 = formatCookie(res.jsmods.require[0][3], "messenger");
        jar.setCookie(cookie, "https://www.facebook.com");
        jar.setCookie(cookie2, "https://www.messenger.com");
      }

      if (res.error === 1357001) {
        throw {error: "Not logged in."};
      }
      return res;
    });
  };
}
```
- example usage
```shell
...
    throw {error: "Elements of userID should be of type Number or String and not " + utils.getType(userID[i]) + "."};
  }

  form['log_message_data[added_participants]['+i+']'] = 'fbid:' + userID[i];
}

defaultFuncs.post("https://www.facebook.com/messaging/send/", ctx.jar, form)
.then(utils.parseAndCheckLogin(ctx.jar, defaultFuncs))
.then(function(resData) {
  if (!resData) {
    throw {error: "Add to group failed."};
  }
  if(resData.error) {
    throw resData;
  }
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.post"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>post (url, jar, form)](#apidoc.element.facebook-chat-api.utils.post)
- description and source-code
```javascript
function post(url, jar, form) {
  var op = {
    headers: getHeaders(url),
    timeout: 60000,
    url: url,
    method: "POST",
    form: form,
    jar: jar,
    gzip: true
  };

  return request(op).then(function(res) {return res[0];});
}
```
- example usage
```shell
...
  var cookieData = JSON.parse("[\"" + utils.getFrom(val, "", "]") + "]");
  jar.setCookie(utils.formatCookie(cookieData, "facebook"), "https://www.facebook.com");
});
// ---------- Very Hacky Part Ends -----------------

log.info("login", "Logging in...");
return utils
  .post("https://www.facebook.com/login.php?login_attempt=1&lwv=110", jar, form)
  .then(utils.saveCookies(jar))
  .then(function(res) {
    var headers = res.headers;
    if (!headers.location) {
      throw {error: "Wrong username/password."};
    }
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.postFormData"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>postFormData (url, jar, form, qs)](#apidoc.element.facebook-chat-api.utils.postFormData)
- description and source-code
```javascript
function postFormData(url, jar, form, qs) {
  var headers = getHeaders(url);
  headers['Content-Type'] = 'multipart/form-data';
  var op = {
    headers: headers,
    timeout: 60000,
    url: url,
    method: "POST",
    formData: form,
    qs: qs,
    jar: jar,
    gzip: true
  };

  return request(op).then(function(res) {return res[0];});
}
```
- example usage
```shell
...

    var form = {
      'images_only': 'true',
      'attachment[]': image,
    };

    uploads.push(defaultFuncs
      .postFormData("https://upload.facebook.com/ajax/mercury/upload.php", ctx.jar, form, {})
      .then(utils.parseAndCheckLogin(ctx.jar, defaultFuncs))
      .then(function (resData) {
if (resData.error) {
  throw resData;
}

return resData.payload.metadata[0];
...
```

#### <a name="apidoc.element.facebook-chat-api.utils.saveCookies"></a>[function <span class="apidocSignatureSpan">facebook-chat-api.utils.</span>saveCookies (jar)](#apidoc.element.facebook-chat-api.utils.saveCookies)
- description and source-code
```javascript
function saveCookies(jar) {
  return function(res) {
    var cookies = res.headers['set-cookie'] || [];
    cookies.forEach(function (c) {
      if (c.indexOf(".facebook.com") > -1) {
        jar.setCookie(c, "https://www.facebook.com");
      }
      var c2 = c.replace(/domain=\.facebook\.com/, "domain=.messenger.com");
      jar.setCookie(c2, "https://www.messenger.com");
    });
    return res;
  };
}
```
- example usage
```shell
...
      jar.setCookie(utils.formatCookie(cookieData, "facebook"), "https://www.facebook.com");
    });
    // ---------- Very Hacky Part Ends -----------------

    log.info("login", "Logging in...");
    return utils
      .post("https://www.facebook.com/login.php?login_attempt=1&lwv=110", jar, form)
      .then(utils.saveCookies(jar))
      .then(function(res) {
var headers = res.headers;
if (!headers.location) {
  throw {error: "Wrong username/password."};
}

// This means the account has login approvals turned on.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
