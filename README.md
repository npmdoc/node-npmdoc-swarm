# api documentation for  [swarm (v0.3.25)](http://github.com/gritzko/swarm)  [![npm package](https://img.shields.io/npm/v/npmdoc-swarm.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-swarm) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-swarm.svg)](https://travis-ci.org/npmdoc/node-npmdoc-swarm)
#### _reactive data sync lib: replicated model for your web app_

[![NPM](https://nodei.co/npm/swarm.png?downloads=true)](https://www.npmjs.com/package/swarm)

[![apidoc](https://npmdoc.github.io/node-npmdoc-swarm/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-swarm_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-swarm/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-swarm/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-swarm/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Victor Grishchenko",
        "email": "victor.grishchenko@gmail.com"
    },
    "browser": "lib/Html5Client.js",
    "bugs": {
        "url": "https://github.com/gritzko/swarm/issues"
    },
    "contributors": [
        {
            "name": "Aleksei Balandin",
            "email": "aleksisha@gmail.com"
        },
        {
            "name": "Andrey Popp",
            "email": "8mayday@gmail.com"
        }
    ],
    "dependencies": {
        "ws": "~0.4.31"
    },
    "description": "_reactive data sync lib: replicated model for your web app_",
    "devDependencies": {
        "browserify": "",
        "istanbul": "^0.3.2",
        "jshint": "",
        "leveldown": "1.0.0",
        "nopt": "",
        "qunit": "^0.7.5"
    },
    "directories": {},
    "dist": {
        "shasum": "5d852f155406e1b9c1162e4a6db8e7c1fa46769e",
        "tarball": "https://registry.npmjs.org/swarm/-/swarm-0.3.25.tgz"
    },
    "email": "swarm.js@gmail.com",
    "files": [
        "lib/*.js",
        "dist/*.js",
        "Makefile",
        "LICENSE"
    ],
    "gitHead": "b945ea204aed653c762e8667e40a1047df2054c2",
    "homepage": "http://github.com/gritzko/swarm",
    "license": "MIT",
    "main": "lib/NodeServer.js",
    "maintainers": [
        {
            "name": "gritzko",
            "email": "victor.grishchenko@gmail.com"
        },
        {
            "name": "abalandin",
            "email": "aleksisha@gmail.com"
        }
    ],
    "name": "swarm",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/gritzko/swarm.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "0.3.25"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module swarm](#apidoc.module.swarm)
1.  [function <span class="apidocSignatureSpan">swarm.</span>EinarosWSStream (ws)](#apidoc.element.swarm.EinarosWSStream)
1.  [function <span class="apidocSignatureSpan">swarm.</span>FileStorage (dir)](#apidoc.element.swarm.FileStorage)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Host (id, ms, storage)](#apidoc.element.swarm.Host)
1.  [function <span class="apidocSignatureSpan">swarm.</span>LamportClock (processId, initTime)](#apidoc.element.swarm.LamportClock)
1.  [function <span class="apidocSignatureSpan">swarm.</span>LevelStorage (id, options, callback)](#apidoc.element.swarm.LevelStorage)
1.  [function <span class="apidocSignatureSpan">swarm.</span>LongSpec (spec, codeBook)](#apidoc.element.swarm.LongSpec)
1.  [function <span class="apidocSignatureSpan">swarm.</span>LongSpec.Iterator (owner, index)](#apidoc.element.swarm.LongSpec.Iterator)
1.  [function <span class="apidocSignatureSpan">swarm.</span>MinutePreciseClock (processId, timeOffsetMs)](#apidoc.element.swarm.MinutePreciseClock)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Model (idOrState)](#apidoc.element.swarm.Model)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Pipe (host, stream, opts)](#apidoc.element.swarm.Pipe)
1.  [function <span class="apidocSignatureSpan">swarm.</span>ProxyListener ()](#apidoc.element.swarm.ProxyListener)
1.  [function <span class="apidocSignatureSpan">swarm.</span>SecondPreciseClock (processId, timeOffsetMs)](#apidoc.element.swarm.SecondPreciseClock)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Set ()](#apidoc.element.swarm.Set)
1.  [function <span class="apidocSignatureSpan">swarm.</span>SharedWebStorage (id, options)](#apidoc.element.swarm.SharedWebStorage)
1.  [function <span class="apidocSignatureSpan">swarm.</span>SockJSServerStream (ws)](#apidoc.element.swarm.SockJSServerStream)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Spec (str, quant)](#apidoc.element.swarm.Spec)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Spec.Map (vec)](#apidoc.element.swarm.Spec.Map)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Storage (async)](#apidoc.element.swarm.Storage)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Syncable ()](#apidoc.element.swarm.Syncable)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Text ()](#apidoc.element.swarm.Text)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Vector ()](#apidoc.element.swarm.Vector)
1.  [function <span class="apidocSignatureSpan">swarm.</span>WebSocketStream (url)](#apidoc.element.swarm.WebSocketStream)
1.  object <span class="apidocSignatureSpan">swarm.</span>CollectionMethodsMixin
1.  object <span class="apidocSignatureSpan">swarm.</span>EinarosWSStream.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>FileStorage.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Host.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Host.prototype._neutrals
1.  object <span class="apidocSignatureSpan">swarm.</span>Host.prototype._ops
1.  object <span class="apidocSignatureSpan">swarm.</span>LamportClock.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>LevelStorage.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>LongSpec.Iterator.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>LongSpec.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>MinutePreciseClock.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Model.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Model.prototype._neutrals
1.  object <span class="apidocSignatureSpan">swarm.</span>Model.prototype._ops
1.  object <span class="apidocSignatureSpan">swarm.</span>Pipe.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>ProxyListener.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>ReactMixin
1.  object <span class="apidocSignatureSpan">swarm.</span>SecondPreciseClock.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Set.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Set.prototype._neutrals
1.  object <span class="apidocSignatureSpan">swarm.</span>Set.prototype._ops
1.  object <span class="apidocSignatureSpan">swarm.</span>SharedWebStorage.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>SockJSServerStream.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Spec.Map.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Spec.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Storage.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Syncable.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Syncable.prototype._neutrals
1.  object <span class="apidocSignatureSpan">swarm.</span>Syncable.prototype._ops
1.  object <span class="apidocSignatureSpan">swarm.</span>Syncable.types
1.  object <span class="apidocSignatureSpan">swarm.</span>Syncable.types.Text.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Vector.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>Vector.prototype._neutrals
1.  object <span class="apidocSignatureSpan">swarm.</span>Vector.prototype._ops
1.  object <span class="apidocSignatureSpan">swarm.</span>env
1.  object <span class="apidocSignatureSpan">swarm.</span>env.streams
1.  object <span class="apidocSignatureSpan">swarm.</span>env.streams.loopback.prototype
1.  object <span class="apidocSignatureSpan">swarm.</span>env.streams.wss.prototype
1.  string <span class="apidocSignatureSpan">swarm.</span>profile

#### [module swarm.CollectionMethodsMixin](#apidoc.module.swarm.CollectionMethodsMixin)
1.  [function <span class="apidocSignatureSpan">swarm.CollectionMethodsMixin.</span>offObjectEvent (callback)](#apidoc.element.swarm.CollectionMethodsMixin.offObjectEvent)
1.  [function <span class="apidocSignatureSpan">swarm.CollectionMethodsMixin.</span>onObjectEvent (callback)](#apidoc.element.swarm.CollectionMethodsMixin.onObjectEvent)
1.  [function <span class="apidocSignatureSpan">swarm.CollectionMethodsMixin.</span>onObjectStateReady (callback)](#apidoc.element.swarm.CollectionMethodsMixin.onObjectStateReady)

#### [module swarm.EinarosWSStream](#apidoc.module.swarm.EinarosWSStream)
1.  [function <span class="apidocSignatureSpan">swarm.</span>EinarosWSStream (ws)](#apidoc.element.swarm.EinarosWSStream.EinarosWSStream)

#### [module swarm.EinarosWSStream.prototype](#apidoc.module.swarm.EinarosWSStream.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.EinarosWSStream.prototype.</span>on (evname, fn)](#apidoc.element.swarm.EinarosWSStream.prototype.on)
1.  [function <span class="apidocSignatureSpan">swarm.EinarosWSStream.prototype.</span>write (data)](#apidoc.element.swarm.EinarosWSStream.prototype.write)

#### [module swarm.FileStorage](#apidoc.module.swarm.FileStorage)
1.  [function <span class="apidocSignatureSpan">swarm.</span>FileStorage (dir)](#apidoc.element.swarm.FileStorage.FileStorage)

#### [module swarm.FileStorage.prototype](#apidoc.module.swarm.FileStorage.prototype)
1.  boolean <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>async
1.  [function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>close (callback, error)](#apidoc.element.swarm.FileStorage.prototype.close)
1.  [function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>loadLog ()](#apidoc.element.swarm.FileStorage.prototype.loadLog)
1.  [function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>logFileName ()](#apidoc.element.swarm.FileStorage.prototype.logFileName)
1.  [function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>readOps (ti, callback)](#apidoc.element.swarm.FileStorage.prototype.readOps)
1.  [function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>readState (ti, callback)](#apidoc.element.swarm.FileStorage.prototype.readState)
1.  [function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>rotateLog (noOpen, callback)](#apidoc.element.swarm.FileStorage.prototype.rotateLog)
1.  [function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>stateFileName (spec)](#apidoc.element.swarm.FileStorage.prototype.stateFileName)
1.  [function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>writeOp (spec, value, cb)](#apidoc.element.swarm.FileStorage.prototype.writeOp)
1.  [function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>writeState (spec, state, cb)](#apidoc.element.swarm.FileStorage.prototype.writeState)
1.  object <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>_host
1.  object <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>counts
1.  object <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>lstn
1.  object <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>states
1.  object <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>tails
1.  string <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>_id

#### [module swarm.Host](#apidoc.module.swarm.Host)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Host (id, ms, storage)](#apidoc.element.swarm.Host.Host)
1.  [function <span class="apidocSignatureSpan">swarm.Host.</span>_super ()](#apidoc.element.swarm.Host._super)
1.  [function <span class="apidocSignatureSpan">swarm.Host.</span>addReaction (op, fn)](#apidoc.element.swarm.Host.addReaction)
1.  [function <span class="apidocSignatureSpan">swarm.Host.</span>extend (fn, own)](#apidoc.element.swarm.Host.extend)
1.  [function <span class="apidocSignatureSpan">swarm.Host.</span>hashDistance (peer, obj)](#apidoc.element.swarm.Host.hashDistance)
1.  [function <span class="apidocSignatureSpan">swarm.Host.</span>removeReaction (handle)](#apidoc.element.swarm.Host.removeReaction)
1.  number <span class="apidocSignatureSpan">swarm.Host.</span>HASH_POINTS
1.  number <span class="apidocSignatureSpan">swarm.Host.</span>MAX_INT
1.  number <span class="apidocSignatureSpan">swarm.Host.</span>MAX_SYNC_TIME
1.  object <span class="apidocSignatureSpan">swarm.Host.</span>_pt
1.  object <span class="apidocSignatureSpan">swarm.Host.</span>defaults

#### [module swarm.Host.prototype](#apidoc.module.swarm.Host.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>accept (stream_or_url, pipe_env)](#apidoc.element.swarm.Host.prototype.accept)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>addSource (spec, peer)](#apidoc.element.swarm.Host.prototype.addSource)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>callReactions (spec, value, src)](#apidoc.element.swarm.Host.prototype.callReactions)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>checkUplink (spec)](#apidoc.element.swarm.Host.prototype.checkUplink)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>close (cb)](#apidoc.element.swarm.Host.prototype.close)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>connect (stream_or_url, pipe_env)](#apidoc.element.swarm.Host.prototype.connect)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>constructor (id, ms, storage)](#apidoc.element.swarm.Host.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>deliver (spec, val, repl)](#apidoc.element.swarm.Host.prototype.deliver)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>disconnect (id)](#apidoc.element.swarm.Host.prototype.disconnect)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>get (spec, callback)](#apidoc.element.swarm.Host.prototype.get)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>getSources (spec)](#apidoc.element.swarm.Host.prototype.getSources)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>init (spec, val, repl)](#apidoc.element.swarm.Host.prototype.init)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>isServer ()](#apidoc.element.swarm.Host.prototype.isServer)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>isUplinked ()](#apidoc.element.swarm.Host.prototype.isUplinked)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>off ()](#apidoc.element.swarm.Host.prototype.off)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>on ()](#apidoc.element.swarm.Host.prototype.on)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>register (obj)](#apidoc.element.swarm.Host.prototype.register)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>removeSource (spec, peer)](#apidoc.element.swarm.Host.prototype.removeSource)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>reoff ()](#apidoc.element.swarm.Host.prototype.reoff)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>reon ()](#apidoc.element.swarm.Host.prototype.reon)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>time ()](#apidoc.element.swarm.Host.prototype.time)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>unregister (obj)](#apidoc.element.swarm.Host.prototype.unregister)
1.  object <span class="apidocSignatureSpan">swarm.Host.prototype.</span>_neutrals
1.  object <span class="apidocSignatureSpan">swarm.Host.prototype.</span>_ops
1.  object <span class="apidocSignatureSpan">swarm.Host.prototype.</span>_reactions
1.  object <span class="apidocSignatureSpan">swarm.Host.prototype.</span>_super
1.  string <span class="apidocSignatureSpan">swarm.Host.prototype.</span>_type

#### [module swarm.Host.prototype._neutrals](#apidoc.module.swarm.Host.prototype._neutrals)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype._neutrals.</span>error (spec, val, repl)](#apidoc.element.swarm.Host.prototype._neutrals.error)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype._neutrals.</span>off (spec, nothing, peer)](#apidoc.element.swarm.Host.prototype._neutrals.off)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype._neutrals.</span>on (spec, filter, lstn)](#apidoc.element.swarm.Host.prototype._neutrals.on)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype._neutrals.</span>reoff (spec, nothing, peer)](#apidoc.element.swarm.Host.prototype._neutrals.reoff)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype._neutrals.</span>reon (spec, ms, host)](#apidoc.element.swarm.Host.prototype._neutrals.reon)

#### [module swarm.Host.prototype._ops](#apidoc.module.swarm.Host.prototype._ops)
1.  [function <span class="apidocSignatureSpan">swarm.Host.prototype._ops.</span>init (spec, state, src)](#apidoc.element.swarm.Host.prototype._ops.init)

#### [module swarm.LamportClock](#apidoc.module.swarm.LamportClock)
1.  [function <span class="apidocSignatureSpan">swarm.</span>LamportClock (processId, initTime)](#apidoc.element.swarm.LamportClock.LamportClock)

#### [module swarm.LamportClock.prototype](#apidoc.module.swarm.LamportClock.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.LamportClock.prototype.</span>adjustTime ()](#apidoc.element.swarm.LamportClock.prototype.adjustTime)
1.  [function <span class="apidocSignatureSpan">swarm.LamportClock.prototype.</span>checkTimestamp (ts)](#apidoc.element.swarm.LamportClock.prototype.checkTimestamp)
1.  [function <span class="apidocSignatureSpan">swarm.LamportClock.prototype.</span>issueTimestamp ()](#apidoc.element.swarm.LamportClock.prototype.issueTimestamp)
1.  [function <span class="apidocSignatureSpan">swarm.LamportClock.prototype.</span>parseTimestamp (ts)](#apidoc.element.swarm.LamportClock.prototype.parseTimestamp)
1.  [function <span class="apidocSignatureSpan">swarm.LamportClock.prototype.</span>time2date ()](#apidoc.element.swarm.LamportClock.prototype.time2date)

#### [module swarm.LevelStorage](#apidoc.module.swarm.LevelStorage)
1.  [function <span class="apidocSignatureSpan">swarm.</span>LevelStorage (id, options, callback)](#apidoc.element.swarm.LevelStorage.LevelStorage)

#### [module swarm.LevelStorage.prototype](#apidoc.module.swarm.LevelStorage.prototype)
1.  boolean <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>async
1.  boolean <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>isRoot
1.  [function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>close (callback, error)](#apidoc.element.swarm.LevelStorage.prototype.close)
1.  [function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>off (spec, val, src)](#apidoc.element.swarm.LevelStorage.prototype.off)
1.  [function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>open (callback)](#apidoc.element.swarm.LevelStorage.prototype.open)
1.  [function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>readOps (ti, callback)](#apidoc.element.swarm.LevelStorage.prototype.readOps)
1.  [function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>readState (ti, callback)](#apidoc.element.swarm.LevelStorage.prototype.readState)
1.  [function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>writeOp (spec, value, cb)](#apidoc.element.swarm.LevelStorage.prototype.writeOp)
1.  [function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>writeState (spec, state, cb)](#apidoc.element.swarm.LevelStorage.prototype.writeState)
1.  object <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>_host
1.  object <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>counts
1.  object <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>lstn
1.  object <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>states
1.  object <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>tails
1.  string <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>_id

#### [module swarm.LongSpec](#apidoc.module.swarm.LongSpec)
1.  [function <span class="apidocSignatureSpan">swarm.</span>LongSpec (spec, codeBook)](#apidoc.element.swarm.LongSpec.LongSpec)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.</span>Iterator (owner, index)](#apidoc.element.swarm.LongSpec.Iterator)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.</span>int2uni (i)](#apidoc.element.swarm.LongSpec.int2uni)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.</span>uni2int (uni)](#apidoc.element.swarm.LongSpec.uni2int)
1.  object <span class="apidocSignatureSpan">swarm.LongSpec.</span>quants2code
1.  object <span class="apidocSignatureSpan">swarm.LongSpec.</span>reQTok
1.  object <span class="apidocSignatureSpan">swarm.LongSpec.</span>reQTokEn
1.  object <span class="apidocSignatureSpan">swarm.LongSpec.</span>reQTokExtEn
1.  string <span class="apidocSignatureSpan">swarm.LongSpec.</span>rTEn

#### [module swarm.LongSpec.Iterator](#apidoc.module.swarm.LongSpec.Iterator)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.</span>Iterator (owner, index)](#apidoc.element.swarm.LongSpec.Iterator.Iterator)
1.  object <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.</span>reTok

#### [module swarm.LongSpec.Iterator.prototype](#apidoc.module.swarm.LongSpec.Iterator.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>clone ()](#apidoc.element.swarm.LongSpec.Iterator.prototype.clone)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>decode ()](#apidoc.element.swarm.LongSpec.Iterator.prototype.decode)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>encode (de)](#apidoc.element.swarm.LongSpec.Iterator.prototype.encode)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>end ()](#apidoc.element.swarm.LongSpec.Iterator.prototype.end)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>erase (count)](#apidoc.element.swarm.LongSpec.Iterator.prototype.erase)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>insert (de)](#apidoc.element.swarm.LongSpec.Iterator.prototype.insert)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>insertBlock (de)](#apidoc.element.swarm.LongSpec.Iterator.prototype.insertBlock)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>next ( )](#apidoc.element.swarm.LongSpec.Iterator.prototype.next)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>skip ( count )](#apidoc.element.swarm.LongSpec.Iterator.prototype.skip)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>skip2chunk ( chunk )](#apidoc.element.swarm.LongSpec.Iterator.prototype.skip2chunk)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>token ()](#apidoc.element.swarm.LongSpec.Iterator.prototype.token)

#### [module swarm.LongSpec.prototype](#apidoc.module.swarm.LongSpec.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>add (spec)](#apidoc.element.swarm.LongSpec.prototype.add)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>allocateCode (tok)](#apidoc.element.swarm.LongSpec.prototype.allocateCode)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>append (spec)](#apidoc.element.swarm.LongSpec.prototype.append)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>charLength ()](#apidoc.element.swarm.LongSpec.prototype.charLength)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>end ()](#apidoc.element.swarm.LongSpec.prototype.end)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>find (tok, startIndex)](#apidoc.element.swarm.LongSpec.prototype.find)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>indexOf (tok, startAt)](#apidoc.element.swarm.LongSpec.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>insert (tok, i)](#apidoc.element.swarm.LongSpec.prototype.insert)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>iterator (index)](#apidoc.element.swarm.LongSpec.prototype.iterator)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>length ()](#apidoc.element.swarm.LongSpec.prototype.length)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>toString ()](#apidoc.element.swarm.LongSpec.prototype.toString)
1.  [function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>tokenAt (pos)](#apidoc.element.swarm.LongSpec.prototype.tokenAt)

#### [module swarm.MinutePreciseClock](#apidoc.module.swarm.MinutePreciseClock)
1.  [function <span class="apidocSignatureSpan">swarm.</span>MinutePreciseClock (processId, timeOffsetMs)](#apidoc.element.swarm.MinutePreciseClock.MinutePreciseClock)
1.  number <span class="apidocSignatureSpan">swarm.MinutePreciseClock.</span>EPOCH

#### [module swarm.MinutePreciseClock.prototype](#apidoc.module.swarm.MinutePreciseClock.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.MinutePreciseClock.prototype.</span>adjustTime (trueMs)](#apidoc.element.swarm.MinutePreciseClock.prototype.adjustTime)
1.  [function <span class="apidocSignatureSpan">swarm.MinutePreciseClock.prototype.</span>checkTimestamp (ts)](#apidoc.element.swarm.MinutePreciseClock.prototype.checkTimestamp)
1.  [function <span class="apidocSignatureSpan">swarm.MinutePreciseClock.prototype.</span>issueTimestamp ()](#apidoc.element.swarm.MinutePreciseClock.prototype.issueTimestamp)
1.  [function <span class="apidocSignatureSpan">swarm.MinutePreciseClock.prototype.</span>minutes ()](#apidoc.element.swarm.MinutePreciseClock.prototype.minutes)
1.  [function <span class="apidocSignatureSpan">swarm.MinutePreciseClock.prototype.</span>parseTimestamp (ts)](#apidoc.element.swarm.MinutePreciseClock.prototype.parseTimestamp)
1.  [function <span class="apidocSignatureSpan">swarm.MinutePreciseClock.prototype.</span>time2date ()](#apidoc.element.swarm.MinutePreciseClock.prototype.time2date)

#### [module swarm.Model](#apidoc.module.swarm.Model)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Model (idOrState)](#apidoc.element.swarm.Model.Model)
1.  [function <span class="apidocSignatureSpan">swarm.Model.</span>_super ()](#apidoc.element.swarm.Model._super)
1.  [function <span class="apidocSignatureSpan">swarm.Model.</span>addReaction (methodOrField, fn)](#apidoc.element.swarm.Model.addReaction)
1.  [function <span class="apidocSignatureSpan">swarm.Model.</span>extend (fn, own)](#apidoc.element.swarm.Model.extend)
1.  [function <span class="apidocSignatureSpan">swarm.Model.</span>removeReaction (handle)](#apidoc.element.swarm.Model.removeReaction)
1.  object <span class="apidocSignatureSpan">swarm.Model.</span>_pt
1.  object <span class="apidocSignatureSpan">swarm.Model.</span>defaults

#### [module swarm.Model.prototype](#apidoc.module.swarm.Model.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>callReactions (spec, value, src)](#apidoc.element.swarm.Model.prototype.callReactions)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>constructor (idOrState)](#apidoc.element.swarm.Model.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>distillLog ()](#apidoc.element.swarm.Model.prototype.distillLog)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>fill (key)](#apidoc.element.swarm.Model.prototype.fill)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>off ()](#apidoc.element.swarm.Model.prototype.off)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>on ()](#apidoc.element.swarm.Model.prototype.on)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>packState (state)](#apidoc.element.swarm.Model.prototype.packState)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>save ()](#apidoc.element.swarm.Model.prototype.save)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>set ()](#apidoc.element.swarm.Model.prototype.set)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>unpackState (state)](#apidoc.element.swarm.Model.prototype.unpackState)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>validate (spec, val)](#apidoc.element.swarm.Model.prototype.validate)
1.  object <span class="apidocSignatureSpan">swarm.Model.prototype.</span>_neutrals
1.  object <span class="apidocSignatureSpan">swarm.Model.prototype.</span>_ops
1.  object <span class="apidocSignatureSpan">swarm.Model.prototype.</span>_reactions
1.  object <span class="apidocSignatureSpan">swarm.Model.prototype.</span>_super
1.  string <span class="apidocSignatureSpan">swarm.Model.prototype.</span>_type

#### [module swarm.Model.prototype._neutrals](#apidoc.module.swarm.Model.prototype._neutrals)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype._neutrals.</span>error (spec, val, repl)](#apidoc.element.swarm.Model.prototype._neutrals.error)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype._neutrals.</span>off (spec, base, repl)](#apidoc.element.swarm.Model.prototype._neutrals.off)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype._neutrals.</span>on (spec, base, repl)](#apidoc.element.swarm.Model.prototype._neutrals.on)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype._neutrals.</span>reoff (spec, val, repl)](#apidoc.element.swarm.Model.prototype._neutrals.reoff)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype._neutrals.</span>reon (spec, filter, repl)](#apidoc.element.swarm.Model.prototype._neutrals.reon)

#### [module swarm.Model.prototype._ops](#apidoc.module.swarm.Model.prototype._ops)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype._ops.</span>init (spec, state, src)](#apidoc.element.swarm.Model.prototype._ops.init)
1.  [function <span class="apidocSignatureSpan">swarm.Model.prototype._ops.</span>set (spec, value, repl)](#apidoc.element.swarm.Model.prototype._ops.set)

#### [module swarm.Pipe](#apidoc.module.swarm.Pipe)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Pipe (host, stream, opts)](#apidoc.element.swarm.Pipe.Pipe)
1.  number <span class="apidocSignatureSpan">swarm.Pipe.</span>TIMEOUT

#### [module swarm.Pipe.prototype](#apidoc.module.swarm.Pipe.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>close (error)](#apidoc.element.swarm.Pipe.prototype.close)
1.  [function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>connect (stream)](#apidoc.element.swarm.Pipe.prototype.connect)
1.  [function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>deliver (spec, val, src)](#apidoc.element.swarm.Pipe.prototype.deliver)
1.  [function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>keepAliveFn ()](#apidoc.element.swarm.Pipe.prototype.keepAliveFn)
1.  [function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>parseBundle (bundle)](#apidoc.element.swarm.Pipe.prototype.parseBundle)
1.  [function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>parseHandshake (handshake)](#apidoc.element.swarm.Pipe.prototype.parseHandshake)
1.  [function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>sendBundle ()](#apidoc.element.swarm.Pipe.prototype.sendBundle)
1.  [function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>spec ()](#apidoc.element.swarm.Pipe.prototype.spec)
1.  [function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>time ()](#apidoc.element.swarm.Pipe.prototype.time)

#### [module swarm.ProxyListener](#apidoc.module.swarm.ProxyListener)
1.  [function <span class="apidocSignatureSpan">swarm.</span>ProxyListener ()](#apidoc.element.swarm.ProxyListener.ProxyListener)

#### [module swarm.ProxyListener.prototype](#apidoc.module.swarm.ProxyListener.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.ProxyListener.prototype.</span>deliver (spec, value, src)](#apidoc.element.swarm.ProxyListener.prototype.deliver)
1.  [function <span class="apidocSignatureSpan">swarm.ProxyListener.prototype.</span>off (callback)](#apidoc.element.swarm.ProxyListener.prototype.off)
1.  [function <span class="apidocSignatureSpan">swarm.ProxyListener.prototype.</span>on (callback)](#apidoc.element.swarm.ProxyListener.prototype.on)

#### [module swarm.ReactMixin](#apidoc.module.swarm.ReactMixin)
1.  [function <span class="apidocSignatureSpan">swarm.ReactMixin.</span>componentWillMount ()](#apidoc.element.swarm.ReactMixin.componentWillMount)
1.  [function <span class="apidocSignatureSpan">swarm.ReactMixin.</span>componentWillUnmount ()](#apidoc.element.swarm.ReactMixin.componentWillUnmount)
1.  [function <span class="apidocSignatureSpan">swarm.ReactMixin.</span>deliver (spec, val, source)](#apidoc.element.swarm.ReactMixin.deliver)
1.  [function <span class="apidocSignatureSpan">swarm.ReactMixin.</span>shouldComponentUpdate (nextProps, nextState)](#apidoc.element.swarm.ReactMixin.shouldComponentUpdate)

#### [module swarm.SecondPreciseClock](#apidoc.module.swarm.SecondPreciseClock)
1.  [function <span class="apidocSignatureSpan">swarm.</span>SecondPreciseClock (processId, timeOffsetMs)](#apidoc.element.swarm.SecondPreciseClock.SecondPreciseClock)
1.  number <span class="apidocSignatureSpan">swarm.SecondPreciseClock.</span>EPOCH

#### [module swarm.SecondPreciseClock.prototype](#apidoc.module.swarm.SecondPreciseClock.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>adjustTime (trueMs)](#apidoc.element.swarm.SecondPreciseClock.prototype.adjustTime)
1.  [function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>checkTimestamp (ts)](#apidoc.element.swarm.SecondPreciseClock.prototype.checkTimestamp)
1.  [function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>issueTimestamp ()](#apidoc.element.swarm.SecondPreciseClock.prototype.issueTimestamp)
1.  [function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>ms ()](#apidoc.element.swarm.SecondPreciseClock.prototype.ms)
1.  [function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>parseTimestamp (ts)](#apidoc.element.swarm.SecondPreciseClock.prototype.parseTimestamp)
1.  [function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>seconds ()](#apidoc.element.swarm.SecondPreciseClock.prototype.seconds)
1.  [function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>timestamp2date (ts)](#apidoc.element.swarm.SecondPreciseClock.prototype.timestamp2date)

#### [module swarm.Set](#apidoc.module.swarm.Set)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Set ()](#apidoc.element.swarm.Set.Set)
1.  [function <span class="apidocSignatureSpan">swarm.Set.</span>_super ()](#apidoc.element.swarm.Set._super)
1.  [function <span class="apidocSignatureSpan">swarm.Set.</span>addReaction (op, fn)](#apidoc.element.swarm.Set.addReaction)
1.  [function <span class="apidocSignatureSpan">swarm.Set.</span>extend (fn, own)](#apidoc.element.swarm.Set.extend)
1.  [function <span class="apidocSignatureSpan">swarm.Set.</span>removeReaction (handle)](#apidoc.element.swarm.Set.removeReaction)
1.  object <span class="apidocSignatureSpan">swarm.Set.</span>_pt
1.  object <span class="apidocSignatureSpan">swarm.Set.</span>defaults

#### [module swarm.Set.prototype](#apidoc.module.swarm.Set.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>addObject (obj)](#apidoc.element.swarm.Set.prototype.addObject)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>callReactions (spec, value, src)](#apidoc.element.swarm.Set.prototype.callReactions)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>change ()](#apidoc.element.swarm.Set.prototype.change)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>constructor ()](#apidoc.element.swarm.Set.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>distillLog ()](#apidoc.element.swarm.Set.prototype.distillLog)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>distillOp (spec, val)](#apidoc.element.swarm.Set.prototype.distillOp)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>every (cb, thisArg)](#apidoc.element.swarm.Set.prototype.every)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>filter (cb, thisArg)](#apidoc.element.swarm.Set.prototype.filter)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>forEach (cb, thisArg)](#apidoc.element.swarm.Set.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>get (key_spec)](#apidoc.element.swarm.Set.prototype.get)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>list (order)](#apidoc.element.swarm.Set.prototype.list)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>map (cb, thisArg)](#apidoc.element.swarm.Set.prototype.map)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>offObjectEvent (callback)](#apidoc.element.swarm.Set.prototype.offObjectEvent)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>onObjectEvent (callback)](#apidoc.element.swarm.Set.prototype.onObjectEvent)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>onObjectStateReady (callback)](#apidoc.element.swarm.Set.prototype.onObjectStateReady)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>pojo ()](#apidoc.element.swarm.Set.prototype.pojo)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>removeObject (obj)](#apidoc.element.swarm.Set.prototype.removeObject)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>validate (spec, val, src)](#apidoc.element.swarm.Set.prototype.validate)
1.  object <span class="apidocSignatureSpan">swarm.Set.prototype.</span>_neutrals
1.  object <span class="apidocSignatureSpan">swarm.Set.prototype.</span>_ops
1.  object <span class="apidocSignatureSpan">swarm.Set.prototype.</span>_reactions
1.  object <span class="apidocSignatureSpan">swarm.Set.prototype.</span>_super
1.  string <span class="apidocSignatureSpan">swarm.Set.prototype.</span>_type

#### [module swarm.Set.prototype._neutrals](#apidoc.module.swarm.Set.prototype._neutrals)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype._neutrals.</span>error (spec, val, repl)](#apidoc.element.swarm.Set.prototype._neutrals.error)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype._neutrals.</span>off (spec, val, repl)](#apidoc.element.swarm.Set.prototype._neutrals.off)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype._neutrals.</span>on (spec, filter, repl)](#apidoc.element.swarm.Set.prototype._neutrals.on)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype._neutrals.</span>reoff (spec, val, repl)](#apidoc.element.swarm.Set.prototype._neutrals.reoff)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype._neutrals.</span>reon (spec, filter, repl)](#apidoc.element.swarm.Set.prototype._neutrals.reon)

#### [module swarm.Set.prototype._ops](#apidoc.module.swarm.Set.prototype._ops)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype._ops.</span>change (spec, value, repl)](#apidoc.element.swarm.Set.prototype._ops.change)
1.  [function <span class="apidocSignatureSpan">swarm.Set.prototype._ops.</span>init (spec, state, src)](#apidoc.element.swarm.Set.prototype._ops.init)

#### [module swarm.SharedWebStorage](#apidoc.module.swarm.SharedWebStorage)
1.  [function <span class="apidocSignatureSpan">swarm.</span>SharedWebStorage (id, options)](#apidoc.element.swarm.SharedWebStorage.SharedWebStorage)

#### [module swarm.SharedWebStorage.prototype](#apidoc.module.swarm.SharedWebStorage.prototype)
1.  boolean <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>async
1.  boolean <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>isRoot
1.  [function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>installListeners ()](#apidoc.element.swarm.SharedWebStorage.prototype.installListeners)
1.  [function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>loadLog ()](#apidoc.element.swarm.SharedWebStorage.prototype.loadLog)
1.  [function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>onOp (spec, value)](#apidoc.element.swarm.SharedWebStorage.prototype.onOp)
1.  [function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>readOps (ti, callback)](#apidoc.element.swarm.SharedWebStorage.prototype.readOps)
1.  [function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>readState (spec, callback)](#apidoc.element.swarm.SharedWebStorage.prototype.readState)
1.  [function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>writeOp (spec, value, src)](#apidoc.element.swarm.SharedWebStorage.prototype.writeOp)
1.  [function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>writeState (spec, state, src)](#apidoc.element.swarm.SharedWebStorage.prototype.writeState)
1.  object <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>_host
1.  object <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>counts
1.  object <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>lstn
1.  object <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>states
1.  object <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>tails
1.  string <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>_id

#### [module swarm.SockJSServerStream](#apidoc.module.swarm.SockJSServerStream)
1.  [function <span class="apidocSignatureSpan">swarm.</span>SockJSServerStream (ws)](#apidoc.element.swarm.SockJSServerStream.SockJSServerStream)

#### [module swarm.SockJSServerStream.prototype](#apidoc.module.swarm.SockJSServerStream.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.SockJSServerStream.prototype.</span>on (evname, fn)](#apidoc.element.swarm.SockJSServerStream.prototype.on)
1.  [function <span class="apidocSignatureSpan">swarm.SockJSServerStream.prototype.</span>write (data)](#apidoc.element.swarm.SockJSServerStream.prototype.write)

#### [module swarm.Spec](#apidoc.module.swarm.Spec)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Spec (str, quant)](#apidoc.element.swarm.Spec.Spec)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.</span>Map (vec)](#apidoc.element.swarm.Spec.Map)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.</span>as (spec)](#apidoc.element.swarm.Spec.as)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.</span>base2int (base)](#apidoc.element.swarm.Spec.base2int)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.</span>int2base (i, padlen)](#apidoc.element.swarm.Spec.int2base)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.</span>is (str)](#apidoc.element.swarm.Spec.is)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.</span>parseToken (token_body)](#apidoc.element.swarm.Spec.parseToken)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.</span>pattern (spec)](#apidoc.element.swarm.Spec.pattern)
1.  object <span class="apidocSignatureSpan">swarm.Spec.</span>quants
1.  object <span class="apidocSignatureSpan">swarm.Spec.</span>re64l
1.  object <span class="apidocSignatureSpan">swarm.Spec.</span>reQTokExt
1.  object <span class="apidocSignatureSpan">swarm.Spec.</span>reTok
1.  object <span class="apidocSignatureSpan">swarm.Spec.</span>reTokExt
1.  string <span class="apidocSignatureSpan">swarm.Spec.</span>base64
1.  string <span class="apidocSignatureSpan">swarm.Spec.</span>rT
1.  string <span class="apidocSignatureSpan">swarm.Spec.</span>rsQTokExt
1.  string <span class="apidocSignatureSpan">swarm.Spec.</span>rsTokExt

#### [module swarm.Spec.Map](#apidoc.module.swarm.Spec.Map)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.</span>Map (vec)](#apidoc.element.swarm.Spec.Map.Map)

#### [module swarm.Spec.Map.prototype](#apidoc.module.swarm.Spec.Map.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.Map.prototype.</span>add (versionVector)](#apidoc.element.swarm.Spec.Map.prototype.add)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.Map.prototype.</span>covers (version)](#apidoc.element.swarm.Spec.Map.prototype.covers)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.Map.prototype.</span>maxTs ()](#apidoc.element.swarm.Spec.Map.prototype.maxTs)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.Map.prototype.</span>toString (trim)](#apidoc.element.swarm.Spec.Map.prototype.toString)

#### [module swarm.Spec.prototype](#apidoc.module.swarm.Spec.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>add (spec, quant)](#apidoc.element.swarm.Spec.prototype.add)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>filter (quants)](#apidoc.element.swarm.Spec.prototype.filter)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>fits (specFilter)](#apidoc.element.swarm.Spec.prototype.fits)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>get (quant)](#apidoc.element.swarm.Spec.prototype.get)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>has (quant)](#apidoc.element.swarm.Spec.prototype.has)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>id ()](#apidoc.element.swarm.Spec.prototype.id)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>isEmpty ()](#apidoc.element.swarm.Spec.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>op ()](#apidoc.element.swarm.Spec.prototype.op)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>pattern ()](#apidoc.element.swarm.Spec.prototype.pattern)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>set (spec, quant)](#apidoc.element.swarm.Spec.prototype.set)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>sort ()](#apidoc.element.swarm.Spec.prototype.sort)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>source ()](#apidoc.element.swarm.Spec.prototype.source)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>toString ()](#apidoc.element.swarm.Spec.prototype.toString)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>tok (quant)](#apidoc.element.swarm.Spec.prototype.tok)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>token (quant)](#apidoc.element.swarm.Spec.prototype.token)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>type ()](#apidoc.element.swarm.Spec.prototype.type)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>typeid ()](#apidoc.element.swarm.Spec.prototype.typeid)
1.  [function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>version ()](#apidoc.element.swarm.Spec.prototype.version)

#### [module swarm.Storage](#apidoc.module.swarm.Storage)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Storage (async)](#apidoc.element.swarm.Storage.Storage)

#### [module swarm.Storage.prototype](#apidoc.module.swarm.Storage.prototype)
1.  boolean <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>isRoot
1.  [function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>anyOp (spec, value, src)](#apidoc.element.swarm.Storage.prototype.anyOp)
1.  [function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>close (callback)](#apidoc.element.swarm.Storage.prototype.close)
1.  [function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>deliver (spec, value, src)](#apidoc.element.swarm.Storage.prototype.deliver)
1.  [function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>emit (spec, value)](#apidoc.element.swarm.Storage.prototype.emit)
1.  [function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>init (spec, state, src)](#apidoc.element.swarm.Storage.prototype.init)
1.  [function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>off (spec, value, src)](#apidoc.element.swarm.Storage.prototype.off)
1.  [function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>on (spec, base, src)](#apidoc.element.swarm.Storage.prototype.on)
1.  [function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>readOps (ti, callback)](#apidoc.element.swarm.Storage.prototype.readOps)
1.  [function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>readState (ti, callback)](#apidoc.element.swarm.Storage.prototype.readState)
1.  [function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>writeOp (spec, value, cb)](#apidoc.element.swarm.Storage.prototype.writeOp)
1.  [function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>writeState (spec, state, cb)](#apidoc.element.swarm.Storage.prototype.writeState)
1.  number <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>MAX_LOG_SIZE

#### [module swarm.Syncable](#apidoc.module.swarm.Syncable)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Syncable ()](#apidoc.element.swarm.Syncable.Syncable)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.</span>_super ()](#apidoc.element.swarm.Syncable._super)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.</span>addReaction (op, fn)](#apidoc.element.swarm.Syncable.addReaction)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.</span>extend (fn, own)](#apidoc.element.swarm.Syncable.extend)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.</span>isOpSink (obj)](#apidoc.element.swarm.Syncable.isOpSink)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.</span>listenerEquals (ln, other)](#apidoc.element.swarm.Syncable.listenerEquals)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.</span>removeReaction (handle)](#apidoc.element.swarm.Syncable.removeReaction)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.</span>stateVersionVector (state)](#apidoc.element.swarm.Syncable.stateVersionVector)
1.  object <span class="apidocSignatureSpan">swarm.Syncable.</span>_default
1.  object <span class="apidocSignatureSpan">swarm.Syncable.</span>_pt
1.  object <span class="apidocSignatureSpan">swarm.Syncable.</span>defaults
1.  object <span class="apidocSignatureSpan">swarm.Syncable.</span>memberClasses
1.  object <span class="apidocSignatureSpan">swarm.Syncable.</span>reFieldName
1.  object <span class="apidocSignatureSpan">swarm.Syncable.</span>reMethodName
1.  object <span class="apidocSignatureSpan">swarm.Syncable.</span>types

#### [module swarm.Syncable.prototype](#apidoc.module.swarm.Syncable.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>acl (spec, val, src)](#apidoc.element.swarm.Syncable.prototype.acl)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>apply (values)](#apidoc.element.swarm.Syncable.prototype.apply)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>callReactions (spec, value, src)](#apidoc.element.swarm.Syncable.prototype.callReactions)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>checkUplink ()](#apidoc.element.swarm.Syncable.prototype.checkUplink)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>close ()](#apidoc.element.swarm.Syncable.prototype.close)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>constructor ()](#apidoc.element.swarm.Syncable.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>deliver (spec, value, lstn)](#apidoc.element.swarm.Syncable.prototype.deliver)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>diff (base)](#apidoc.element.swarm.Syncable.prototype.diff)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>distillLog ()](#apidoc.element.swarm.Syncable.prototype.distillLog)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>emit (spec, value, src)](#apidoc.element.swarm.Syncable.prototype.emit)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>error ()](#apidoc.element.swarm.Syncable.prototype.error)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>gc ()](#apidoc.element.swarm.Syncable.prototype.gc)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>getListenerIndex (search_for, uplinks_only)](#apidoc.element.swarm.Syncable.prototype.getListenerIndex)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>hasState ()](#apidoc.element.swarm.Syncable.prototype.hasState)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>init ()](#apidoc.element.swarm.Syncable.prototype.init)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>isReplay (spec)](#apidoc.element.swarm.Syncable.prototype.isReplay)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>newEventSpec (op)](#apidoc.element.swarm.Syncable.prototype.newEventSpec)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>off ()](#apidoc.element.swarm.Syncable.prototype.off)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>on ()](#apidoc.element.swarm.Syncable.prototype.on)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>once (filter, cb)](#apidoc.element.swarm.Syncable.prototype.once)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>pojo (addVersionInfo)](#apidoc.element.swarm.Syncable.prototype.pojo)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>reoff ()](#apidoc.element.swarm.Syncable.prototype.reoff)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>reon ()](#apidoc.element.swarm.Syncable.prototype.reon)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>reset ()](#apidoc.element.swarm.Syncable.prototype.reset)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>spec ()](#apidoc.element.swarm.Syncable.prototype.spec)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>stateSpec ()](#apidoc.element.swarm.Syncable.prototype.stateSpec)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>trigger (event, params)](#apidoc.element.swarm.Syncable.prototype.trigger)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>unimplemented (spec, val, repl)](#apidoc.element.swarm.Syncable.prototype.unimplemented)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>validate (spec, val, src)](#apidoc.element.swarm.Syncable.prototype.validate)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>version ()](#apidoc.element.swarm.Syncable.prototype.version)
1.  object <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>_neutrals
1.  object <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>_ops
1.  object <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>_reactions
1.  object <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>_super
1.  string <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>_type

#### [module swarm.Syncable.prototype._neutrals](#apidoc.module.swarm.Syncable.prototype._neutrals)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype._neutrals.</span>error (spec, val, repl)](#apidoc.element.swarm.Syncable.prototype._neutrals.error)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype._neutrals.</span>off (spec, val, repl)](#apidoc.element.swarm.Syncable.prototype._neutrals.off)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype._neutrals.</span>on (spec, filter, repl)](#apidoc.element.swarm.Syncable.prototype._neutrals.on)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype._neutrals.</span>reoff (spec, val, repl)](#apidoc.element.swarm.Syncable.prototype._neutrals.reoff)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype._neutrals.</span>reon (spec, filter, repl)](#apidoc.element.swarm.Syncable.prototype._neutrals.reon)

#### [module swarm.Syncable.prototype._ops](#apidoc.module.swarm.Syncable.prototype._ops)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.prototype._ops.</span>init (spec, state, src)](#apidoc.element.swarm.Syncable.prototype._ops.init)

#### [module swarm.Syncable.types](#apidoc.module.swarm.Syncable.types)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.</span>Host (id, ms, storage)](#apidoc.element.swarm.Syncable.types.Host)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.</span>Model (idOrState)](#apidoc.element.swarm.Syncable.types.Model)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.</span>Set ()](#apidoc.element.swarm.Syncable.types.Set)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.</span>Syncable ()](#apidoc.element.swarm.Syncable.types.Syncable)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.</span>Text ()](#apidoc.element.swarm.Syncable.types.Text)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.</span>Vector ()](#apidoc.element.swarm.Syncable.types.Vector)

#### [module swarm.Syncable.types.Text.prototype](#apidoc.module.swarm.Syncable.types.Text.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>callReactions (spec, value, src)](#apidoc.element.swarm.Syncable.types.Text.prototype.callReactions)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>constructor ()](#apidoc.element.swarm.Syncable.types.Text.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>insert ()](#apidoc.element.swarm.Syncable.types.Text.prototype.insert)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>rebuild ()](#apidoc.element.swarm.Syncable.types.Text.prototype.rebuild)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>remove ()](#apidoc.element.swarm.Syncable.types.Text.prototype.remove)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>set (newText)](#apidoc.element.swarm.Syncable.types.Text.prototype.set)
1.  [function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>state ()](#apidoc.element.swarm.Syncable.types.Text.prototype.state)
1.  object <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>_neutrals
1.  object <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>_ops
1.  object <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>_reactions
1.  object <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>_super
1.  string <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>_type

#### [module swarm.Text](#apidoc.module.swarm.Text)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Text ()](#apidoc.element.swarm.Text.Text)
1.  [function <span class="apidocSignatureSpan">swarm.Text.</span>_super ()](#apidoc.element.swarm.Text._super)
1.  [function <span class="apidocSignatureSpan">swarm.Text.</span>addReaction (op, fn)](#apidoc.element.swarm.Text.addReaction)
1.  [function <span class="apidocSignatureSpan">swarm.Text.</span>diff (was, is)](#apidoc.element.swarm.Text.diff)
1.  [function <span class="apidocSignatureSpan">swarm.Text.</span>extend (fn, own)](#apidoc.element.swarm.Text.extend)
1.  [function <span class="apidocSignatureSpan">swarm.Text.</span>removeReaction (handle)](#apidoc.element.swarm.Text.removeReaction)
1.  object <span class="apidocSignatureSpan">swarm.Text.</span>_pt
1.  object <span class="apidocSignatureSpan">swarm.Text.</span>defaults

#### [module swarm.Vector](#apidoc.module.swarm.Vector)
1.  [function <span class="apidocSignatureSpan">swarm.</span>Vector ()](#apidoc.element.swarm.Vector.Vector)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.</span>_super ()](#apidoc.element.swarm.Vector._super)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.</span>addReaction (op, fn)](#apidoc.element.swarm.Vector.addReaction)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.</span>extend (fn, own)](#apidoc.element.swarm.Vector.extend)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.</span>removeReaction (handle)](#apidoc.element.swarm.Vector.removeReaction)
1.  object <span class="apidocSignatureSpan">swarm.Vector.</span>_pt
1.  object <span class="apidocSignatureSpan">swarm.Vector.</span>defaults

#### [module swarm.Vector.prototype](#apidoc.module.swarm.Vector.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>addObject (obj)](#apidoc.element.swarm.Vector.prototype.addObject)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>append (spec)](#apidoc.element.swarm.Vector.prototype.append)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>callReactions (spec, value, src)](#apidoc.element.swarm.Vector.prototype.callReactions)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>constructor ()](#apidoc.element.swarm.Vector.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>distillLog ()](#apidoc.element.swarm.Vector.prototype.distillLog)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>every (cb, thisArg)](#apidoc.element.swarm.Vector.prototype.every)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>filter (cb, thisArg)](#apidoc.element.swarm.Vector.prototype.filter)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>findPositionFor (id, parentId)](#apidoc.element.swarm.Vector.prototype.findPositionFor)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>forEach (cb, thisArg)](#apidoc.element.swarm.Vector.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>getObject (spec)](#apidoc.element.swarm.Vector.prototype.getObject)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>getParentOf (id)](#apidoc.element.swarm.Vector.prototype.getParentOf)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>in ()](#apidoc.element.swarm.Vector.prototype.in)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>inSubtreeOf (nodeId, rootId)](#apidoc.element.swarm.Vector.prototype.inSubtreeOf)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>indexOf (obj, startAt)](#apidoc.element.swarm.Vector.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>insert (spec, pos)](#apidoc.element.swarm.Vector.prototype.insert)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>insertAfter (obj, pos)](#apidoc.element.swarm.Vector.prototype.insertAfter)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>insertBefore (spec, pos)](#apidoc.element.swarm.Vector.prototype.insertBefore)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>insertSorted (obj, cmp)](#apidoc.element.swarm.Vector.prototype.insertSorted)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>isDescendantOf (nodeId, rootId)](#apidoc.element.swarm.Vector.prototype.isDescendantOf)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>length ()](#apidoc.element.swarm.Vector.prototype.length)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>map (cb, thisArg)](#apidoc.element.swarm.Vector.prototype.map)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>normalizePos (pos)](#apidoc.element.swarm.Vector.prototype.normalizePos)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>objectAt (i)](#apidoc.element.swarm.Vector.prototype.objectAt)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>offObjectEvent (callback)](#apidoc.element.swarm.Vector.prototype.offObjectEvent)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>onObjectEvent (callback)](#apidoc.element.swarm.Vector.prototype.onObjectEvent)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>onObjectStateReady (callback)](#apidoc.element.swarm.Vector.prototype.onObjectStateReady)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>pojo ()](#apidoc.element.swarm.Vector.prototype.pojo)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>remove (pos)](#apidoc.element.swarm.Vector.prototype.remove)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>removeObject (pos)](#apidoc.element.swarm.Vector.prototype.removeObject)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>rm ()](#apidoc.element.swarm.Vector.prototype.rm)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>setOrder (fn)](#apidoc.element.swarm.Vector.prototype.setOrder)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>skipSubtree (iter, root)](#apidoc.element.swarm.Vector.prototype.skipSubtree)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>validate (spec, val, source)](#apidoc.element.swarm.Vector.prototype.validate)
1.  object <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>_neutrals
1.  object <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>_ops
1.  object <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>_reactions
1.  object <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>_super
1.  string <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>_type

#### [module swarm.Vector.prototype._neutrals](#apidoc.module.swarm.Vector.prototype._neutrals)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype._neutrals.</span>error (spec, val, repl)](#apidoc.element.swarm.Vector.prototype._neutrals.error)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype._neutrals.</span>off (spec, val, repl)](#apidoc.element.swarm.Vector.prototype._neutrals.off)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype._neutrals.</span>on (spec, filter, repl)](#apidoc.element.swarm.Vector.prototype._neutrals.on)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype._neutrals.</span>reoff (spec, val, repl)](#apidoc.element.swarm.Vector.prototype._neutrals.reoff)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype._neutrals.</span>reon (spec, filter, repl)](#apidoc.element.swarm.Vector.prototype._neutrals.reon)

#### [module swarm.Vector.prototype._ops](#apidoc.module.swarm.Vector.prototype._ops)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype._ops.</span>in (spec, value, src)](#apidoc.element.swarm.Vector.prototype._ops.in)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype._ops.</span>init (spec, state, src)](#apidoc.element.swarm.Vector.prototype._ops.init)
1.  [function <span class="apidocSignatureSpan">swarm.Vector.prototype._ops.</span>rm (spec, value, src)](#apidoc.element.swarm.Vector.prototype._ops.rm)

#### [module swarm.WebSocketStream](#apidoc.module.swarm.WebSocketStream)
1.  [function <span class="apidocSignatureSpan">swarm.</span>WebSocketStream (url)](#apidoc.element.swarm.WebSocketStream.WebSocketStream)

#### [module swarm.env](#apidoc.module.swarm.env)
1.  boolean <span class="apidocSignatureSpan">swarm.env.</span>debug
1.  boolean <span class="apidocSignatureSpan">swarm.env.</span>isBrowser
1.  boolean <span class="apidocSignatureSpan">swarm.env.</span>isGecko
1.  boolean <span class="apidocSignatureSpan">swarm.env.</span>isIE
1.  boolean <span class="apidocSignatureSpan">swarm.env.</span>isServer
1.  boolean <span class="apidocSignatureSpan">swarm.env.</span>isWebKit
1.  boolean <span class="apidocSignatureSpan">swarm.env.</span>multihost
1.  boolean <span class="apidocSignatureSpan">swarm.env.</span>trace
1.  [function <span class="apidocSignatureSpan">swarm.env.</span>hashfn (key, seed)](#apidoc.element.swarm.env.hashfn)
1.  [function <span class="apidocSignatureSpan">swarm.env.</span>log (spec, val, object)](#apidoc.element.swarm.env.log)
1.  object <span class="apidocSignatureSpan">swarm.env.</span>streams

#### [module swarm.env.streams](#apidoc.module.swarm.env.streams)
1.  [function <span class="apidocSignatureSpan">swarm.env.streams.</span>loopback (url)](#apidoc.element.swarm.env.streams.loopback)
1.  [function <span class="apidocSignatureSpan">swarm.env.streams.</span>ws (url)](#apidoc.element.swarm.env.streams.ws)
1.  [function <span class="apidocSignatureSpan">swarm.env.streams.</span>wss (url)](#apidoc.element.swarm.env.streams.wss)

#### [module swarm.env.streams.loopback.prototype](#apidoc.module.swarm.env.streams.loopback.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.env.streams.loopback.prototype.</span>close ()](#apidoc.element.swarm.env.streams.loopback.prototype.close)
1.  [function <span class="apidocSignatureSpan">swarm.env.streams.loopback.prototype.</span>on (evname, fn)](#apidoc.element.swarm.env.streams.loopback.prototype.on)
1.  [function <span class="apidocSignatureSpan">swarm.env.streams.loopback.prototype.</span>pair ()](#apidoc.element.swarm.env.streams.loopback.prototype.pair)
1.  [function <span class="apidocSignatureSpan">swarm.env.streams.loopback.prototype.</span>receive (string)](#apidoc.element.swarm.env.streams.loopback.prototype.receive)
1.  [function <span class="apidocSignatureSpan">swarm.env.streams.loopback.prototype.</span>write (obj)](#apidoc.element.swarm.env.streams.loopback.prototype.write)

#### [module swarm.env.streams.wss.prototype](#apidoc.module.swarm.env.streams.wss.prototype)
1.  [function <span class="apidocSignatureSpan">swarm.env.streams.wss.prototype.</span>on (evname, fn)](#apidoc.element.swarm.env.streams.wss.prototype.on)
1.  [function <span class="apidocSignatureSpan">swarm.env.streams.wss.prototype.</span>write (data)](#apidoc.element.swarm.env.streams.wss.prototype.write)



# <a name="apidoc.module.swarm"></a>[module swarm](#apidoc.module.swarm)

#### <a name="apidoc.element.swarm.EinarosWSStream"></a>[function <span class="apidocSignatureSpan">swarm.</span>EinarosWSStream (ws)](#apidoc.element.swarm.EinarosWSStream)
- description and source-code
```javascript
function EinarosWSStream(ws) {
    var self = this,
        ln = this.lstn = {},
        buf = [];

    if (typeof ws === 'string') { // url passed
        ws = new ws_lib(ws);
    }
    this.ws = ws;
    if (ws.readyState !== 1/*WebSocket.OPEN*/) {
        this.buf = buf; //will wait for "open"
    }
    ws.on('open', function () {
        buf.reverse();
        self.buf = null;
        while (buf.length) {
            self.write(buf.pop());
        }
    });
    ws.on('close', function () { ln.close && ln.close(); });
    ws.on('message', function (msg) {
        try {
            ln.data && ln.data(msg);
        } catch (ex) {
            console.error('message processing fails', ex);
            ln.error && ln.error(ex.message);
        }
    });
    ws.on('error', function (msg) { ln.error && ln.error(msg); });
}
```
- example usage
```shell
...

// start WebSocket server
var wsServer = new ws_lib.Server({ server: httpServer });

// accept incoming WebSockets connections
wsServer.on('connection', function (ws) {
    console.log('new incoming WebSocket connection');
    swarmHost.accept(new Swarm.EinarosWSStream(ws), { delay: 50 });
});
'''

see [swarm-example](https://github.com/swarmjs/swarm-example/blob/master/server.js) for a nice example of a generic model sync server


## Swarm API Quickstart
...
```

#### <a name="apidoc.element.swarm.FileStorage"></a>[function <span class="apidocSignatureSpan">swarm.</span>FileStorage (dir)](#apidoc.element.swarm.FileStorage)
- description and source-code
```javascript
function FileStorage(dir) {
    Storage.call(this);
    this._host = null; //will be set during Host creation
    this.dir = path.resolve(dir);
    if (!fs.existsSync(this.dir)) {
        fs.mkdirSync(this.dir);
    }
    this._id = 'file';
    this.tail = {};

    this.loadLog();
    this.rotateLog();
}
```
- example usage
```shell
...

// npm install swarm
var Swarm = require('swarm');

var Mouse = require('./Mouse.js'); // see the model definition above

// use file storage
var fileStorage = new Swarm.FileStorage('storage');

// create the server-side Swarm Host
var swarmHost = new Swarm.Host('swarm~nodejs', 0, fileStorage);

// create and start the HTTP server
var httpServer = http.createServer();
httpServer.listen(8000, function (err) {
...
```

#### <a name="apidoc.element.swarm.Host"></a>[function <span class="apidocSignatureSpan">swarm.</span>Host (id, ms, storage)](#apidoc.element.swarm.Host)
- description and source-code
```javascript
function Host(id, ms, storage) {
    this.objects = {};
    this.sources = {};
    this.storage = storage;
    this._host = this; // :)
    this._lstn = [','];
    this._id = id;
    this._server = /^swarm~.*/.test(id);
    var clock_fn = env.clockType || SecondPreciseClock;
    this.clock = new clock_fn(this._id, ms||0);

    if (this.storage) {
        this.sources[this._id] = this.storage;
        this.storage._host = this;
    }
    delete this.objects[this.spec()];

    if (!env.multihost) {
        if (env.localhost) {
            throw new Error('use multihost mode');
        }
        env.localhost = this;
    }
}
```
- example usage
```shell
...
module.exports = Mouse; // CommonJS
'''

### Using the model on the client (app.js)

'''js
// 1. create local Host
var swarmHost = new Swarm.Host('unique_client_id');

// 2. connect to your server
swarmHost.connect('ws://localhost:8000/');

// 3.a. create an object
var someMouse = new Mouse();
// OR swarmHost.get('/Mouse');
...
```

#### <a name="apidoc.element.swarm.LamportClock"></a>[function <span class="apidocSignatureSpan">swarm.</span>LamportClock (processId, initTime)](#apidoc.element.swarm.LamportClock)
- description and source-code
```javascript
LamportClock = function (processId, initTime) {
    if (!Spec.reTok.test(processId)) {
        throw new Error('invalid process id: '+processId);
    }
    this.id = processId;
    // sometimes we assume our local clock has some offset
    this.seq = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LevelStorage"></a>[function <span class="apidocSignatureSpan">swarm.</span>LevelStorage (id, options, callback)](#apidoc.element.swarm.LevelStorage)
- description and source-code
```javascript
function LevelStorage(id, options, callback) {
    Storage.call(this);
    this.options = options;
    this._host = null; // will be set by the Host
    this.db = options.db;
    this._id = id;
    this.filename = null;
    if (this.db.constructor===Function) {
        this.db = this.db(options.path||id);
    }
    this.logtails = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec"></a>[function <span class="apidocSignatureSpan">swarm.</span>LongSpec (spec, codeBook)](#apidoc.element.swarm.LongSpec)
- description and source-code
```javascript
LongSpec = function (spec, codeBook) {
    var cb = this.codeBook = codeBook || {en:{},de:{}};
    if (!cb.en) { cb.en = {}; }
    if (!cb.de) { // revert en to make de
        cb.de = {};
        for(var tok in cb.en) {
            cb.de[cb.en[tok]] = tok;
        }
    }
    if (!cb.lastCodes) {
        cb.lastCodes = {'/':0x30,'#':0x30,'!':0x30,'.':0x30,'+':0x30};
    }
    // For a larger document, a single LongSpec may be some megabytes long.
    // As we don't want to rewrite those megabytes on every keypress, we
    // divide data into chunks.
    this.chunks = [];
    this.chunkLengths = [];
    if (spec) {
        this.append(spec);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.Iterator"></a>[function <span class="apidocSignatureSpan">swarm.</span>LongSpec.Iterator (owner, index)](#apidoc.element.swarm.LongSpec.Iterator)
- description and source-code
```javascript
function Iterator(owner, index) {
    this.owner = owner;         // our LongSpec
<span class="apidocCodeCommentSpan">    /*this.chunk = 0;             // the chunk we are in
    this.index = -1;            // token index (position "before the 1st token")
    this.chunkIndex = -1;       // token index within the chunk
    this.prevFull = undefined;  // previous full (non-collapsed) token
    //  seqStart IS the previous match or prev match is trivial
    this.prevCollapsed = 0;
    this.match = null;
    //this.next();*/
</span>    this.skip2chunk(0);
    if (index) {
        if (index.constructor===LongSpec.Iterator) {
            index = index.index;
        }
        this.skip(index);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.MinutePreciseClock"></a>[function <span class="apidocSignatureSpan">swarm.</span>MinutePreciseClock (processId, timeOffsetMs)](#apidoc.element.swarm.MinutePreciseClock)
- description and source-code
```javascript
MinutePreciseClock = function (processId, timeOffsetMs) {
    if (!Spec.reTok.test(processId)) {
        throw new Error('invalid process id: '+processId);
    }
    this.id = processId;
    // sometimes we assume our local clock has some offset
    this.clockOffsetMs = 0;
    this.lastIssuedTimestamp = '';
    // although we try hard to use wall clock time, we must
    // obey Lamport logical clock rules, in particular our
    // timestamps must be greater than any other timestamps
    // previously seen
    this.lastTimeSeen = 0;
    this.lastSeqSeen = 0;
    if (timeOffsetMs) {
        this.clockOffsetMs = timeOffsetMs;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model"></a>[function <span class="apidocSignatureSpan">swarm.</span>Model (idOrState)](#apidoc.element.swarm.Model)
- description and source-code
```javascript
function Model(idOrState) {
    var ret = Model._super.apply(this, arguments);
    /// TODO: combine with state push, make clean
    if (ret === this && idOrState && idOrState.constructor !== String && !Spec.is(idOrState)) {
        this.deliver(this.spec().add(this._id, '!').add('.set'), idOrState);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Pipe"></a>[function <span class="apidocSignatureSpan">swarm.</span>Pipe (host, stream, opts)](#apidoc.element.swarm.Pipe)
- description and source-code
```javascript
function Pipe(host, stream, opts) {
    var self = this;
    self.opts = opts || {};
    if (!stream || !host) {
        throw new Error('new Pipe(host,stream[,opts])');
    }
    self._id = null;
    self.host = host;
    // uplink/downlink state flag;
    //  true: this side initiated handshake >.on <.reon
    //  false: this side received handshake <.on >.reon
    //  undefined: nothing sent/received OR had a .reoff
    this.isOnSent = undefined;
    this.reconnectDelay = self.opts.reconnectDelay || 1000;
    self.serializer = self.opts.serializer || JSON;
    self.katimer = null;
    self.send_timer = null;
    self.lastSendTS = self.lastRecvTS = self.time();
    self.bundle = {};
    // don't send immediately, delay to bundle more messages
    self.delay = self.opts.delay || -1;
    //self.reconnectDelay = self.opts.reconnectDelay || 1000;
    if (typeof(stream.write) !== 'function') { // TODO nicer
        var url = stream.toString();
        var m = url.match(/(\w+):.*/);
        if (!m) {
            throw new Error('invalid url ' + url);
        }
        var proto = m[1].toLowerCase();
        var fn = env.streams[proto];
        if (!fn) {
            throw new Error('protocol not supported: ' + proto);
        }
        self.url = url;
        stream = new fn(url);
    }
    self.connect(stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.ProxyListener"></a>[function <span class="apidocSignatureSpan">swarm.</span>ProxyListener ()](#apidoc.element.swarm.ProxyListener)
- description and source-code
```javascript
function ProxyListener() {
    this.callbacks = null;
    this.owner = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.SecondPreciseClock"></a>[function <span class="apidocSignatureSpan">swarm.</span>SecondPreciseClock (processId, timeOffsetMs)](#apidoc.element.swarm.SecondPreciseClock)
- description and source-code
```javascript
SecondPreciseClock = function (processId, timeOffsetMs) {
    if (!Spec.reTok.test(processId)) {
        throw new Error('invalid process id: '+processId);
    }
    this.id = processId;
    // sometimes we assume our local clock has some offset
    this.clockOffsetMs = 0;
    this.lastTimestamp = '';
    // although we try hard to use wall clock time, we must
    // obey Lamport logical clock rules, in particular our
    // timestamps must be greater than any other timestamps
    // previously seen
    this.lastTimeSeen = 0;
    this.lastSeqSeen = 0;
    if (timeOffsetMs) {
        this.clockOffsetMs = timeOffsetMs;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set"></a>[function <span class="apidocSignatureSpan">swarm.</span>Set ()](#apidoc.element.swarm.Set)
- description and source-code
```javascript
function SomeSyncable() {
    return parent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.SharedWebStorage"></a>[function <span class="apidocSignatureSpan">swarm.</span>SharedWebStorage (id, options)](#apidoc.element.swarm.SharedWebStorage)
- description and source-code
```javascript
function SharedWebStorage(id, options) {
    this.options = options || {};
    this.lstn = {};
    this._id = id;
    this.tails = {};
    this.store = this.options.persistent ?
        window.localStorage : window.sessionStorage;

    this.loadLog();
    this.installListeners();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.SockJSServerStream"></a>[function <span class="apidocSignatureSpan">swarm.</span>SockJSServerStream (ws)](#apidoc.element.swarm.SockJSServerStream)
- description and source-code
```javascript
function SockJSStream(ws) {
    var ln = this.lstn = {},
        buf = [];

    if (typeof ws === 'string') { // url passed
        throw new Error('client-side connections not supported yet');
    }
    this.ws = ws;
    if (ws.readyState !== 1/*WebSocket.OPEN*/) {
        this.buf = buf; //will wait for "open"
    }
    ws.on('close', function () { ln.close && ln.close(); });
    ws.on('data', function (msg) {
        try {
            ln.data && ln.data(msg);
        } catch (ex) {
            console.error('message processing fails', ex);
            ln.error && ln.error(ex.message);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec"></a>[function <span class="apidocSignatureSpan">swarm.</span>Spec (str, quant)](#apidoc.element.swarm.Spec)
- description and source-code
```javascript
function Spec(str, quant) {
    if (str && str.constructor === Spec) {
        str = str.value;
    } else { // later we assume value has valid format
        str = (str || '').toString();
        if (quant && str.charAt(0) >= '0') {
            str = quant + str;
        }
        if (str.replace(Spec.reQTokExt, '')) {
            throw new Error('malformed specifier: ' + str);
        }
    }
    this.value = str;
    this.index = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.Map"></a>[function <span class="apidocSignatureSpan">swarm.</span>Spec.Map (vec)](#apidoc.element.swarm.Spec.Map)
- description and source-code
```javascript
function VersionVectorAsAMap(vec) {
    this.map = {};
    if (vec) {
        this.add(vec);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Storage"></a>[function <span class="apidocSignatureSpan">swarm.</span>Storage (async)](#apidoc.element.swarm.Storage)
- description and source-code
```javascript
function Storage(async) {
    this.async = !!async || false;
    this.states = {};
    this.tails = {};
    this.counts = {};
    this._host = null;
    // many implementations do not push changes
    // so there are no listeners
    this.lstn = null;
    this._id = 'some_storage';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable"></a>[function <span class="apidocSignatureSpan">swarm.</span>Syncable ()](#apidoc.element.swarm.Syncable)
- description and source-code
```javascript
function Syncable() {
    // listeners represented as objects that have deliver() method
    this._lstn = [',']; // we unshift() uplink listeners and push() downlinks
    // ...so _lstn is like [server1, server2, storage, ',', view, listener]
    // The most correct way to specify a version is the version vector,
    // but that one may consume more space than the data itself in some cases.
    // Hence, _version is not a fully specified version vector (see version()
    // instead). _version is essentially is the greatest operation timestamp
    // (Lamport-like, i.e. "time+source"), sometimes amended with additional
    // timestamps. Its main features:
    // (1) changes once the object's state changes
    // (2) does it monotonically (in the alphanum order sense)
    this._version = '';
    // make sense of arguments
    var args = Array.prototype.slice.call(arguments);
    this._host = (args.length && args[args.length - 1]._type === 'Host') ?
            args.pop() : env.localhost;
    if (Spec.is(args[0])) {
        this._id = new Spec(args.shift()).id() || this._host.time();
    } else if (typeof(args[0]) === 'string') {
        this._id = args.shift(); // TODO format
    } else {
        this._id = this._host.time();
        this._version = '!0'; // may apply state in the constructor, see Model
    }
    //var state = args.length ? args.pop() : (fresh?{}:undefined);
    // register with the host
    var doubl = this._host.register(this);
    if (doubl !== this) { return doubl; }
    // locally created objects get state immediately
    // (while external-id objects need to query uplinks)
<span class="apidocCodeCommentSpan">    /*if (fresh && state) {
     state._version = '!'+this._id;
     var pspec = this.spec().add(state._version).add('.init');
     this.deliver(pspec,state,this._host);
     }*/
</span>    this.reset();
    // find uplinks, subscribe
    this.checkUplink();
    // TODO inplement state push
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Text"></a>[function <span class="apidocSignatureSpan">swarm.</span>Text ()](#apidoc.element.swarm.Text)
- description and source-code
```javascript
function SomeSyncable() {
    return parent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector"></a>[function <span class="apidocSignatureSpan">swarm.</span>Vector ()](#apidoc.element.swarm.Vector)
- description and source-code
```javascript
function SomeSyncable() {
    return parent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.WebSocketStream"></a>[function <span class="apidocSignatureSpan">swarm.</span>WebSocketStream (url)](#apidoc.element.swarm.WebSocketStream)
- description and source-code
```javascript
function WebSocketStream(url) {
    var self = this;
    var ln = this.lstn = {};
    this.url = url;
    var ws = this.ws = new WebSocket(url);
    var buf = this.buf = [];
    ws.onopen = function () {
        buf.reverse();
        self.buf = null;
        while (buf.length) {
            self.write(buf.pop());
        }

    };
    ws.onclose = function () { ln.close && ln.close(); };
    ws.onmessage = function (msg) {
        ln.data && ln.data(msg.data);
    };
    ws.onerror = function (err) { ln.error && ln.error(err); };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.CollectionMethodsMixin"></a>[module swarm.CollectionMethodsMixin](#apidoc.module.swarm.CollectionMethodsMixin)

#### <a name="apidoc.element.swarm.CollectionMethodsMixin.offObjectEvent"></a>[function <span class="apidocSignatureSpan">swarm.CollectionMethodsMixin.</span>offObjectEvent (callback)](#apidoc.element.swarm.CollectionMethodsMixin.offObjectEvent)
- description and source-code
```javascript
offObjectEvent = function (callback) {
    this._proxy.off(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.CollectionMethodsMixin.onObjectEvent"></a>[function <span class="apidocSignatureSpan">swarm.CollectionMethodsMixin.</span>onObjectEvent (callback)](#apidoc.element.swarm.CollectionMethodsMixin.onObjectEvent)
- description and source-code
```javascript
onObjectEvent = function (callback) {
    this._proxy.owner = this;
    this._proxy.on(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.CollectionMethodsMixin.onObjectStateReady"></a>[function <span class="apidocSignatureSpan">swarm.CollectionMethodsMixin.</span>onObjectStateReady (callback)](#apidoc.element.swarm.CollectionMethodsMixin.onObjectStateReady)
- description and source-code
```javascript
onObjectStateReady = function (callback) { // TODO timeout ?
    var self = this;
    function checker() {
        var notInitedYet = self.filter(function (entry) {
            return !entry._version;
        });
        if (!notInitedYet.length) {
            // all entries are inited
            callback();
        } else {
            // wait for some entry not ready yet
            var randomIdx = (Math.random() * (notInitedYet.length - 1)) | 0;
            notInitedYet[randomIdx].once('init', checker);
        }
    }
    if (this._version) {
        checker();
    } else {
        this.once('init', checker);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.EinarosWSStream"></a>[module swarm.EinarosWSStream](#apidoc.module.swarm.EinarosWSStream)

#### <a name="apidoc.element.swarm.EinarosWSStream.EinarosWSStream"></a>[function <span class="apidocSignatureSpan">swarm.</span>EinarosWSStream (ws)](#apidoc.element.swarm.EinarosWSStream.EinarosWSStream)
- description and source-code
```javascript
function EinarosWSStream(ws) {
    var self = this,
        ln = this.lstn = {},
        buf = [];

    if (typeof ws === 'string') { // url passed
        ws = new ws_lib(ws);
    }
    this.ws = ws;
    if (ws.readyState !== 1/*WebSocket.OPEN*/) {
        this.buf = buf; //will wait for "open"
    }
    ws.on('open', function () {
        buf.reverse();
        self.buf = null;
        while (buf.length) {
            self.write(buf.pop());
        }
    });
    ws.on('close', function () { ln.close && ln.close(); });
    ws.on('message', function (msg) {
        try {
            ln.data && ln.data(msg);
        } catch (ex) {
            console.error('message processing fails', ex);
            ln.error && ln.error(ex.message);
        }
    });
    ws.on('error', function (msg) { ln.error && ln.error(msg); });
}
```
- example usage
```shell
...

// start WebSocket server
var wsServer = new ws_lib.Server({ server: httpServer });

// accept incoming WebSockets connections
wsServer.on('connection', function (ws) {
    console.log('new incoming WebSocket connection');
    swarmHost.accept(new Swarm.EinarosWSStream(ws), { delay: 50 });
});
'''

see [swarm-example](https://github.com/swarmjs/swarm-example/blob/master/server.js) for a nice example of a generic model sync server


## Swarm API Quickstart
...
```



# <a name="apidoc.module.swarm.EinarosWSStream.prototype"></a>[module swarm.EinarosWSStream.prototype](#apidoc.module.swarm.EinarosWSStream.prototype)

#### <a name="apidoc.element.swarm.EinarosWSStream.prototype.on"></a>[function <span class="apidocSignatureSpan">swarm.EinarosWSStream.prototype.</span>on (evname, fn)](#apidoc.element.swarm.EinarosWSStream.prototype.on)
- description and source-code
```javascript
on = function (evname, fn) {
    if (evname in this.lstn) {
        throw new Error('not supported');
    }
    this.lstn[evname] = fn;
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.EinarosWSStream.prototype.write"></a>[function <span class="apidocSignatureSpan">swarm.EinarosWSStream.prototype.</span>write (data)](#apidoc.element.swarm.EinarosWSStream.prototype.write)
- description and source-code
```javascript
write = function (data) {
    if (this.buf) {
        this.buf.push(data.toString());
    } else {
        this.ws.send(data.toString());
    }
}
```
- example usage
```shell
...
    this.queue = [];
    if (this.id in AsyncLoopbackConnection.pipes) {
        throw new Error('duplicate');
    }
    AsyncLoopbackConnection.pipes[this.id] = this;
    var pair = this.pair();
    if (pair && pair.queue.length) {
        pair.write();
    }
}
AsyncLoopbackConnection.pipes = {};

env.streams.loopback = AsyncLoopbackConnection;

AsyncLoopbackConnection.prototype.pair = function () {
...
```



# <a name="apidoc.module.swarm.FileStorage"></a>[module swarm.FileStorage](#apidoc.module.swarm.FileStorage)

#### <a name="apidoc.element.swarm.FileStorage.FileStorage"></a>[function <span class="apidocSignatureSpan">swarm.</span>FileStorage (dir)](#apidoc.element.swarm.FileStorage.FileStorage)
- description and source-code
```javascript
function FileStorage(dir) {
    Storage.call(this);
    this._host = null; //will be set during Host creation
    this.dir = path.resolve(dir);
    if (!fs.existsSync(this.dir)) {
        fs.mkdirSync(this.dir);
    }
    this._id = 'file';
    this.tail = {};

    this.loadLog();
    this.rotateLog();
}
```
- example usage
```shell
...

// npm install swarm
var Swarm = require('swarm');

var Mouse = require('./Mouse.js'); // see the model definition above

// use file storage
var fileStorage = new Swarm.FileStorage('storage');

// create the server-side Swarm Host
var swarmHost = new Swarm.Host('swarm~nodejs', 0, fileStorage);

// create and start the HTTP server
var httpServer = http.createServer();
httpServer.listen(8000, function (err) {
...
```



# <a name="apidoc.module.swarm.FileStorage.prototype"></a>[module swarm.FileStorage.prototype](#apidoc.module.swarm.FileStorage.prototype)

#### <a name="apidoc.element.swarm.FileStorage.prototype.close"></a>[function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>close (callback, error)](#apidoc.element.swarm.FileStorage.prototype.close)
- description and source-code
```javascript
close = function (callback, error) {
    if (error) {
        console.log("fatal IO error", error);
    }
    if (this.logFile) {
        this.rotateLog(true, callback);
    }
}
```
- example usage
```shell
...
        }
    }, 1);
};

AsyncLoopbackConnection.prototype.close = function () {
    delete AsyncLoopbackConnection.pipes[this.id];
    var pair = this.pair();
    pair && pair.close();
    this.lstn.close && this.lstn.close();
};
...
```

#### <a name="apidoc.element.swarm.FileStorage.prototype.loadLog"></a>[function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>loadLog ()](#apidoc.element.swarm.FileStorage.prototype.loadLog)
- description and source-code
```javascript
loadLog = function () {
    if ( !fs.existsSync(this.logFileName()) ) {
        return;
    }
    var json = fs.readFileSync(this.logFileName(), {encoding:"utf8"});
    if (!json) { return; }
    var log;
    try {
        log = JSON.parse(json);
    } catch (ex) {
        // open-ended JSON
        log = JSON.parse(json + '}');
    }
    this.tails = log[''];
    delete log[''];
    for(var s in log) {
        var spec = new Spec(s);
        if (spec.pattern()==='/#!.') {
            var ti = spec.filter('/#');
            var vm = spec.filter('!.');
            var tail = this.tails[ti] || (this.tails[ti] = {});
            tail[vm]  = log[spec];
        }
    }
}
```
- example usage
```shell
...
    this.options = options || {};
    this.lstn = {};
    this._id = id;
    this.tails = {};
    this.store = this.options.persistent ?
        window.localStorage : window.sessionStorage;

    this.loadLog();
    this.installListeners();
}

SharedWebStorage.prototype = new Storage();
SharedWebStorage.prototype.isRoot = false;
module.exports = SharedWebStorage;
...
```

#### <a name="apidoc.element.swarm.FileStorage.prototype.logFileName"></a>[function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>logFileName ()](#apidoc.element.swarm.FileStorage.prototype.logFileName)
- description and source-code
```javascript
logFileName = function () {
    return path.resolve(this.dir, "_log");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.FileStorage.prototype.readOps"></a>[function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>readOps (ti, callback)](#apidoc.element.swarm.FileStorage.prototype.readOps)
- description and source-code
```javascript
readOps = function (ti, callback) {
    var tail = this.tails[ti];
    if (tail) {
        var unjsoned = {};
        for(var key in tail) {
            unjsoned[key] = tail[key];
        }
        tail = unjsoned;
    }
    callback(null, tail||null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.FileStorage.prototype.readState"></a>[function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>readState (ti, callback)](#apidoc.element.swarm.FileStorage.prototype.readState)
- description and source-code
```javascript
readState = function (ti, callback) {
    var statefn = this.stateFileName(ti);
    // read in the state
    fs.readFile(statefn, function onRead(err, data) { // FIXME fascism
        var state = err ? {_version: '!0'} : JSON.parse(data.toString());
        callback(null,state||null); // important: no state is "null"
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.FileStorage.prototype.rotateLog"></a>[function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>rotateLog (noOpen, callback)](#apidoc.element.swarm.FileStorage.prototype.rotateLog)
- description and source-code
```javascript
rotateLog = function (noOpen, callback) {
    var self = this;
    if (this.logFile) {
        this.logFile.end('}', callback);
        this.logFile = null;
        callback = undefined;
    }

    if (!noOpen) {

        if (fs.existsSync(this.logFileName())) {
            fs.rename(this.logFileName(),this.logFileName()+'.bak');
        }
        this.logFile = fs.createWriteStream(this.logFileName()); // TODO file swap
        this.logFile.on('error', function (err) {
            self.close(null,err);
        });

        var json = JSON.stringify(this.tails, undefined, 2);
        json = '{"":\n' + json; // open-ended JSON

        this.logFile.write (json, function onFail(err) {
            if (err) { self.close(null,err); }
        });

    }

    if (callback) {
        callback();
    }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.FileStorage.prototype.stateFileName"></a>[function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>stateFileName (spec)](#apidoc.element.swarm.FileStorage.prototype.stateFileName)
- description and source-code
```javascript
stateFileName = function (spec) {
    var base = path.resolve(this.dir, spec.type());
    var file = path.resolve(base, spec.id());
    return file; // TODO hashing?
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.FileStorage.prototype.writeOp"></a>[function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>writeOp (spec, value, cb)](#apidoc.element.swarm.FileStorage.prototype.writeOp)
- description and source-code
```javascript
writeOp = function (spec, value, cb) {
    var self = this;
    var ti = spec.filter('/#');
    var vm = spec.filter('!.');
    var tail = this.tails[ti] || (this.tails[ti] = {});
    if (vm in tail) {
        console.error('op replay @storage',vm,new Error().stack);
        return;
    }
    var clone = JSON.parse(JSON.stringify(value)); // FIXME performance please
    tail[vm] = clone;
    var record = ',\n"'+spec+'":\t'+JSON.stringify(clone);
    this.logFile.write (record, function onFail(err) {
        if (err) { self.close(null,err); }
        cb(err);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.FileStorage.prototype.writeState"></a>[function <span class="apidocSignatureSpan">swarm.FileStorage.prototype.</span>writeState (spec, state, cb)](#apidoc.element.swarm.FileStorage.prototype.writeState)
- description and source-code
```javascript
writeState = function (spec, state, cb) {
    var self = this;
    var ti = spec.filter('/#');
    var fileName = this.stateFileName(ti);
    var dir = path.dirname(fileName);
    if (!fs.existsSync(dir)) {
        fs.mkdirSync(dir);
    }
    var save = JSON.stringify(state, undefined, 2);
    // dump JSON to the tmp file
    delete self.tails[ti]; // TODO save 'em in case write fails
    fs.writeFile(fileName, save, function onSave(err) {
        if (err) {
            console.error("failed to flush state; can't trim the log", err);
        }
        cb(err);
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Host"></a>[module swarm.Host](#apidoc.module.swarm.Host)

#### <a name="apidoc.element.swarm.Host.Host"></a>[function <span class="apidocSignatureSpan">swarm.</span>Host (id, ms, storage)](#apidoc.element.swarm.Host.Host)
- description and source-code
```javascript
function Host(id, ms, storage) {
    this.objects = {};
    this.sources = {};
    this.storage = storage;
    this._host = this; // :)
    this._lstn = [','];
    this._id = id;
    this._server = /^swarm~.*/.test(id);
    var clock_fn = env.clockType || SecondPreciseClock;
    this.clock = new clock_fn(this._id, ms||0);

    if (this.storage) {
        this.sources[this._id] = this.storage;
        this.storage._host = this;
    }
    delete this.objects[this.spec()];

    if (!env.multihost) {
        if (env.localhost) {
            throw new Error('use multihost mode');
        }
        env.localhost = this;
    }
}
```
- example usage
```shell
...
module.exports = Mouse; // CommonJS
'''

### Using the model on the client (app.js)

'''js
// 1. create local Host
var swarmHost = new Swarm.Host('unique_client_id');

// 2. connect to your server
swarmHost.connect('ws://localhost:8000/');

// 3.a. create an object
var someMouse = new Mouse();
// OR swarmHost.get('/Mouse');
...
```

#### <a name="apidoc.element.swarm.Host._super"></a>[function <span class="apidocSignatureSpan">swarm.Host.</span>_super ()](#apidoc.element.swarm.Host._super)
- description and source-code
```javascript
function Syncable() {
    // listeners represented as objects that have deliver() method
    this._lstn = [',']; // we unshift() uplink listeners and push() downlinks
    // ...so _lstn is like [server1, server2, storage, ',', view, listener]
    // The most correct way to specify a version is the version vector,
    // but that one may consume more space than the data itself in some cases.
    // Hence, _version is not a fully specified version vector (see version()
    // instead). _version is essentially is the greatest operation timestamp
    // (Lamport-like, i.e. "time+source"), sometimes amended with additional
    // timestamps. Its main features:
    // (1) changes once the object's state changes
    // (2) does it monotonically (in the alphanum order sense)
    this._version = '';
    // make sense of arguments
    var args = Array.prototype.slice.call(arguments);
    this._host = (args.length && args[args.length - 1]._type === 'Host') ?
            args.pop() : env.localhost;
    if (Spec.is(args[0])) {
        this._id = new Spec(args.shift()).id() || this._host.time();
    } else if (typeof(args[0]) === 'string') {
        this._id = args.shift(); // TODO format
    } else {
        this._id = this._host.time();
        this._version = '!0'; // may apply state in the constructor, see Model
    }
    //var state = args.length ? args.pop() : (fresh?{}:undefined);
    // register with the host
    var doubl = this._host.register(this);
    if (doubl !== this) { return doubl; }
    // locally created objects get state immediately
    // (while external-id objects need to query uplinks)
<span class="apidocCodeCommentSpan">    /*if (fresh && state) {
     state._version = '!'+this._id;
     var pspec = this.spec().add(state._version).add('.init');
     this.deliver(pspec,state,this._host);
     }*/
</span>    this.reset();
    // find uplinks, subscribe
    this.checkUplink();
    // TODO inplement state push
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.addReaction"></a>[function <span class="apidocSignatureSpan">swarm.Host.</span>addReaction (op, fn)](#apidoc.element.swarm.Host.addReaction)
- description and source-code
```javascript
addReaction = function (op, fn) {
    var reactions = this.prototype._reactions;
    var list = reactions[op];
    list || (list = reactions[op] = []);
    list.push(fn);
    return {op: op, fn: fn};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.extend"></a>[function <span class="apidocSignatureSpan">swarm.Host.</span>extend (fn, own)](#apidoc.element.swarm.Host.extend)
- description and source-code
```javascript
extend = function (fn, own) {
    var parent = this, fnid;
    if (fn.constructor !== Function) {
        var id = fn.toString();
        fn = function SomeSyncable() {
            return parent.apply(this, arguments);
        };
        fnid = id; // if only it worked
    } else { // please call Syncable.constructor.apply(this,args) in your constructor
        fnid = fnname(fn);
    }

    // inheritance trick from backbone.js
    var SyncProto = function () {
        this.constructor = fn;
        this._neutrals = {};
        this._ops = {};
        this._reactions = {};

        var event,
            name;
        if (parent._pt) {
            //copy _neutrals & _ops from parent
            for (event in parent._pt._neutrals) {
                this._neutrals[event] = parent._pt._neutrals[event];
            }
            for (event in parent._pt._ops) {
                this._ops[event] = parent._pt._ops[event];
            }
        }

        // "Methods" are serialized, logged and delivered to replicas
        for (name in own.ops || {}) {
            if (Syncable.reMethodName.test(name)) {
                this._ops[name] = own.ops[name];
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid op name:',name);
            }
        }

        // "Neutrals" don't change the state
        for (name in own.neutrals || {}) {
            if (Syncable.reMethodName.test(name)) {
                this._neutrals[name] = own.neutrals[name];
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid neutral op name:',name);
            }
        }

        // "Remotes" are serialized and sent upstream (like RPC calls)
        for (name in own.remotes || {}) {
            if (Syncable.reMethodName.test(name)) {
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid rpc name:',name);
            }
        }

        // add mixins
        (own.mixins || []).forEach(function (mixin) {
            for (var name in mixin) {
                this[name] = mixin[name];
            }
        }, this);

        // add other members
        for (name in own) {
            if (Syncable.reMethodName.test(name)) {
                var memberType = own[name].constructor;
                if (memberType === Function) { // non-op method
                    // these must change state ONLY by invoking ops
                    this[name] = own[name];
                } else if (memberType===String || memberType===Number) {
                    this[name] = own[name]; // some static constant, OK
                } else if (name in Syncable.memberClasses) {
                    // see above
                    continue;
                } else {
                    console.warn('invalid member:',name,memberType);
                }
            } else {
                console.warn('invalid member name:',name);
            }
        }

        // add reactions
        for (name in own.reactions || {}) {
            var reaction = own.reactions[name];
            if (!reaction) { continue; }

            switch (typeof reaction) {
            case 'function':
                // handler-function
                this._reactions[name] = [reaction];
                break;
            case 'string':
                // handler-method name
                this._reactions[name] = [this[name]];
                break;
            default:
                if (reaction.constructor === Array) {
                    // array of handlers
                    this._reactions[name] = reaction.map(function (item) {
                        switch (typeof item) {
                        case 'function':
                            return item;
                        case 'string':
                            return this[item];
                        default:
                            throw new Error('unexpected reaction type');
                        }
                    }, this);
                } else {
                    throw new Error('unex ...
```
- example usage
```shell
...
these demos are normally online at http://ppyr.us and http://ppyr.us:8001/demo3/index.html respectively.

### Creating your first simple synchronized type

'''js
var Swarm = require('swarm');

var Mouse = Swarm.Model.extend('Mouse', {
    defaults: {
        name: 'Mickey',
        x: 0,
        y: 0
    }
});
...
```

#### <a name="apidoc.element.swarm.Host.hashDistance"></a>[function <span class="apidocSignatureSpan">swarm.Host.</span>hashDistance (peer, obj)](#apidoc.element.swarm.Host.hashDistance)
- description and source-code
```javascript
function hashDistance(peer, obj) {
    if ((obj).constructor !== Number) {
        if (obj._id) {
            obj = obj._id;
        }
        obj = env.hashfn(obj);
    }
    if (peer._id) {
        peer = peer._id;
    }
    var dist = 4294967295;
    for (var i = 0; i < Host.HASH_POINTS; i++) {
        var hash = env.hashfn(peer._id + ':' + i);
        dist = Math.min(dist, hash ^ obj);
    }
    return dist;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.removeReaction"></a>[function <span class="apidocSignatureSpan">swarm.Host.</span>removeReaction (handle)](#apidoc.element.swarm.Host.removeReaction)
- description and source-code
```javascript
removeReaction = function (handle) {
    var op = handle.op,
        fn = handle.fn,
        list = this.prototype._reactions[op],
        i = list.indexOf(fn);
    if (i === -1) {
        throw new Error('reaction unknown');
    }
    list[i] = undefined; // such a peculiar pattern not to mess up out-of-callback removal
    while (list.length && !list[list.length - 1]) {
        list.pop();
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Host.prototype"></a>[module swarm.Host.prototype](#apidoc.module.swarm.Host.prototype)

#### <a name="apidoc.element.swarm.Host.prototype.accept"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>accept (stream_or_url, pipe_env)](#apidoc.element.swarm.Host.prototype.accept)
- description and source-code
```javascript
accept = function (stream_or_url, pipe_env) {
    new Pipe(this, stream_or_url, pipe_env);
}
```
- example usage
```shell
...

// start WebSocket server
var wsServer = new ws_lib.Server({ server: httpServer });

// accept incoming WebSockets connections
wsServer.on('connection', function (ws) {
    console.log('new incoming WebSocket connection');
    swarmHost.accept(new Swarm.EinarosWSStream(ws), { delay: 50 });
});
'''

see [swarm-example](https://github.com/swarmjs/swarm-example/blob/master/server.js) for a nice example of a generic model sync server


## Swarm API Quickstart
...
```

#### <a name="apidoc.element.swarm.Host.prototype.addSource"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>addSource (spec, peer)](#apidoc.element.swarm.Host.prototype.addSource)
- description and source-code
```javascript
function hostAddPeer(spec, peer) {
    //FIXME when their time is off so tell them so
    // if (false) { this.clockOffset; }
    var old = this.sources[peer._id];
    if (old) {
        old.deliver(this.newEventSpec('off'), '', this);
    }

    this.sources[peer._id] = peer;
    if (spec.op() === 'on') {
        peer.deliver(this.newEventSpec('reon'), this.clock.ms(), this);
    }
    for (var sp in this.objects) {
        this.objects[sp].checkUplink();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.callReactions"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>callReactions (spec, value, src)](#apidoc.element.swarm.Host.prototype.callReactions)
- description and source-code
```javascript
callReactions = function (spec, value, src) {
    var superReactions = syncProto._super.callReactions;
    if ('function' === typeof superReactions) {
        superReactions.call(this, spec, value, src);
    }
    var r = syncProto._reactions[spec.op()];
    if (r) {
        r.constructor !== Array && (r = [r]);
        for (var i = 0; i < r.length; i++) {
            r[i] && r[i].call(this, spec, value, src);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.checkUplink"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>checkUplink (spec)](#apidoc.element.swarm.Host.prototype.checkUplink)
- description and source-code
```javascript
checkUplink = function (spec) {
    //  TBD Host event relay + PEX
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.close"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>close (cb)](#apidoc.element.swarm.Host.prototype.close)
- description and source-code
```javascript
close = function (cb) {
    for(var id in this.sources) {
        if (id===this._id) {continue;}
        this.disconnect(id);
    }
    if (this.storage) {
        this.storage.close(cb);
    } else if (cb) {
        cb();
    }
}
```
- example usage
```shell
...
        }
    }, 1);
};

AsyncLoopbackConnection.prototype.close = function () {
    delete AsyncLoopbackConnection.pipes[this.id];
    var pair = this.pair();
    pair && pair.close();
    this.lstn.close && this.lstn.close();
};
...
```

#### <a name="apidoc.element.swarm.Host.prototype.connect"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>connect (stream_or_url, pipe_env)](#apidoc.element.swarm.Host.prototype.connect)
- description and source-code
```javascript
connect = function (stream_or_url, pipe_env) {
    var pipe = new Pipe(this, stream_or_url, pipe_env);
    pipe.deliver(new Spec('/Host#'+this._id+'!0.on'), '', this); //this.newEventSpec
    return pipe;
}
```
- example usage
```shell
...
### Using the model on the client (app.js)

'''js
// 1. create local Host
var swarmHost = new Swarm.Host('unique_client_id');

// 2. connect to your server
swarmHost.connect('ws://localhost:8000/');

// 3.a. create an object
var someMouse = new Mouse();
// OR swarmHost.get('/Mouse');
// OR new Mouse({x:1, y:2});

// 4.a. a locally created object may be touched immediately
...
```

#### <a name="apidoc.element.swarm.Host.prototype.constructor"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>constructor (id, ms, storage)](#apidoc.element.swarm.Host.prototype.constructor)
- description and source-code
```javascript
function Host(id, ms, storage) {
    this.objects = {};
    this.sources = {};
    this.storage = storage;
    this._host = this; // :)
    this._lstn = [','];
    this._id = id;
    this._server = /^swarm~.*/.test(id);
    var clock_fn = env.clockType || SecondPreciseClock;
    this.clock = new clock_fn(this._id, ms||0);

    if (this.storage) {
        this.sources[this._id] = this.storage;
        this.storage._host = this;
    }
    delete this.objects[this.spec()];

    if (!env.multihost) {
        if (env.localhost) {
            throw new Error('use multihost mode');
        }
        env.localhost = this;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.deliver"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>deliver (spec, val, repl)](#apidoc.element.swarm.Host.prototype.deliver)
- description and source-code
```javascript
deliver = function (spec, val, repl) {
    if (spec.type() !== 'Host') {
        var typeid = spec.filter('/#');
        var obj = this.get(typeid);
        if (obj) {
            // TODO seeTimestamp()
            obj.deliver(spec, val, repl);
        }
    } else {
        this._super.deliver.apply(this, arguments);
    }
}
```
- example usage
```shell
...
if (this.callbacks===null) { return; }
var that = this.owner || src;
for(var i=0; i<this.callbacks.length; i++) {
    var cb = this.callbacks[i];
    if (cb.constructor===Function) {
        cb.call(that,spec,value,src);
    } else {
        cb.deliver(spec,value,src);
    }
}
};

ProxyListener.prototype.on = function (callback) {
if (this.callbacks===null) { this.callbacks = []; }
this.callbacks.push(callback);
...
```

#### <a name="apidoc.element.swarm.Host.prototype.disconnect"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>disconnect (id)](#apidoc.element.swarm.Host.prototype.disconnect)
- description and source-code
```javascript
disconnect = function (id) {
    for (var peer_id in this.sources) {
        if (id && peer_id != id) {
            continue;
        }
        if (peer_id === this._id) {
            // storage
            continue;
        }
        var peer = this.sources[peer_id];
        // normally, .off is sent by a downlink
        peer.deliver(peer.spec().add(this.time(), '!').add('.off'));
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.get"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>get (spec, callback)](#apidoc.element.swarm.Host.prototype.get)
- description and source-code
```javascript
get = function (spec, callback) {
    if (spec && spec.constructor === Function && spec.prototype._type) {
        spec = '/' + spec.prototype._type;
    }
    spec = new Spec(spec);
    var typeid = spec.filter('/#');
    if (!typeid.has('/')) {
        throw new Error('invalid spec');
    }
    var o = typeid.has('#') && this.objects[typeid];
    if (!o) {
        var t = Syncable.types[spec.type()];
        if (!t) {
            throw new Error('type unknown: ' + spec);
        }
        o = new t(typeid, undefined, this);
        if (typeof(callback) === 'function') {
            o.on('.init', callback);
        }
    }
    return o;
}
```
- example usage
```shell
...
var swarmHost = new Swarm.Host('unique_client_id');

// 2. connect to your server
swarmHost.connect('ws://localhost:8000/');

// 3.a. create an object
var someMouse = new Mouse();
// OR swarmHost.get('/Mouse');
// OR new Mouse({x:1, y:2});

// 4.a. a locally created object may be touched immediately
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
...
```

#### <a name="apidoc.element.swarm.Host.prototype.getSources"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>getSources (spec)](#apidoc.element.swarm.Host.prototype.getSources)
- description and source-code
```javascript
getSources = function (spec) {
    var self = this,
        uplinks = [],
        mindist = 4294967295,
        rePeer = /^swarm~/, // peers, not clients
        target = env.hashfn(spec),
        closestPeer = null;

    if (rePeer.test(this._id)) {
        mindist = Host.hashDistance(this._id, target);
        closestPeer = this.storage;
    } else {
        uplinks.push(self.storage); // client-side cache
    }

    for (var id in this.sources) {
        if (!rePeer.test(id)) {
            continue;
        }
        var dist = Host.hashDistance(id, target);
        if (dist < mindist) {
            closestPeer = this.sources[id];
            mindist = dist;
        }
    }
    if (closestPeer) {
        uplinks.push(closestPeer);
    }
    return uplinks;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.init"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>init (spec, val, repl)](#apidoc.element.swarm.Host.prototype.init)
- description and source-code
```javascript
init = function (spec, val, repl) {

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.isServer"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>isServer ()](#apidoc.element.swarm.Host.prototype.isServer)
- description and source-code
```javascript
isServer = function () {
    return this._server;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.isUplinked"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>isUplinked ()](#apidoc.element.swarm.Host.prototype.isUplinked)
- description and source-code
```javascript
isUplinked = function () {
    for (var id in this.sources) {
        if (/^swarm~.*/.test(id)) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.off"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>off ()](#apidoc.element.swarm.Host.prototype.off)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
...

/**
 * Unsubscribe from collections entries' events
 * @param {function(*)} callback
 * @this Set|Vector
 */
offObjectEvent: function (callback) {
    this._proxy.off(callback);
},

/**
 * Waits for collection to receive state from cache or uplink and then invokes passed callback
 *
 * @param {function()} callback
 * @this Set|Vector
...
```

#### <a name="apidoc.element.swarm.Host.prototype.on"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>on ()](#apidoc.element.swarm.Host.prototype.on)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.Host.prototype.register"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>register (obj)](#apidoc.element.swarm.Host.prototype.register)
- description and source-code
```javascript
register = function (obj) {
    var spec = obj.spec();
    if (spec in this.objects) {
        return this.objects[spec];
    }
    this.objects[spec] = obj;
    return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.removeSource"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>removeSource (spec, peer)](#apidoc.element.swarm.Host.prototype.removeSource)
- description and source-code
```javascript
removeSource = function (spec, peer) {
    if (spec.type() !== 'Host') {
        throw new Error('Host.removeSource(/NoHost)');
    }

    if (this.sources[peer._id] !== peer) {
        console.error('peer unknown', peer._id); //throw new Error
        return;
    }
    delete this.sources[peer._id];
    for (var sp in this.objects) {
        var obj = this.objects[sp];
        if (obj.getListenerIndex(peer, true) > -1) {
            obj.off(sp, '', peer);
            obj.checkUplink(sp);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.reoff"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>reoff ()](#apidoc.element.swarm.Host.prototype.reoff)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.reon"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>reon ()](#apidoc.element.swarm.Host.prototype.reon)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.time"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>time ()](#apidoc.element.swarm.Host.prototype.time)
- description and source-code
```javascript
time = function () {
    var ts = this.clock.issueTimestamp();
    this._version = ts;
    return ts;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype.unregister"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype.</span>unregister (obj)](#apidoc.element.swarm.Host.prototype.unregister)
- description and source-code
```javascript
unregister = function (obj) {
    var spec = obj.spec();
    // TODO unsubscribe from the uplink - swarm-scale gc
    if (spec in this.objects) {
        delete this.objects[spec];
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Host.prototype._neutrals"></a>[module swarm.Host.prototype._neutrals](#apidoc.module.swarm.Host.prototype._neutrals)

#### <a name="apidoc.element.swarm.Host.prototype._neutrals.error"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype._neutrals.</span>error (spec, val, repl)](#apidoc.element.swarm.Host.prototype._neutrals.error)
- description and source-code
```javascript
error = function (spec, val, repl) {
    console.error('something failed:', spec, val, '@', (repl && repl._id));
}
```
- example usage
```shell
...
        this.buf = buf; //will wait for "open"
    }
    ws.on('close', function () { ln.close && ln.close(); });
    ws.on('data', function (msg) {
        try {
            ln.data && ln.data(msg);
        } catch (ex) {
            console.error('message processing fails', ex);
            ln.error && ln.error(ex.message);
        }
    });
}

module.exports = SockJSStream;
...
```

#### <a name="apidoc.element.swarm.Host.prototype._neutrals.off"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype._neutrals.</span>off (spec, nothing, peer)](#apidoc.element.swarm.Host.prototype._neutrals.off)
- description and source-code
```javascript
off = function (spec, nothing, peer) {
    peer.deliver(peer.spec().add(this.time(), '!').add('.reoff'), '', this);
    this.removeSource(spec, peer);
}
```
- example usage
```shell
...

/**
 * Unsubscribe from collections entries' events
 * @param {function(*)} callback
 * @this Set|Vector
 */
offObjectEvent: function (callback) {
    this._proxy.off(callback);
},

/**
 * Waits for collection to receive state from cache or uplink and then invokes passed callback
 *
 * @param {function()} callback
 * @this Set|Vector
...
```

#### <a name="apidoc.element.swarm.Host.prototype._neutrals.on"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype._neutrals.</span>on (spec, filter, lstn)](#apidoc.element.swarm.Host.prototype._neutrals.on)
- description and source-code
```javascript
function hostOn(spec, filter, lstn) {
    if (!filter) {
        // the subscriber needs "all the events"
        return this.addSource(spec, lstn);
    }

    if (filter.constructor === Function && filter.id) {
        filter = new Spec(filter.id, '/');
    } else if (filter.constructor === String) {
        filter = new Spec(filter, '.');
    }
    // either suscribe to this Host or to some other object
    if (!filter.has('/') || filter.type() === 'Host') {
        this._super._neutrals.on.call(this, spec, filter, lstn);
    } else {
        var objSpec = new Spec(filter);
        if (!objSpec.has('#')) {
            throw new Error('no id to listen');
        }
        objSpec = objSpec.set('.on').set(spec.version(), '!');
        this.deliver(objSpec, filter, lstn);
    }
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.Host.prototype._neutrals.reoff"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype._neutrals.</span>reoff (spec, nothing, peer)](#apidoc.element.swarm.Host.prototype._neutrals.reoff)
- description and source-code
```javascript
function hostReOff(spec, nothing, peer) {
    this.removeSource(spec, peer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Host.prototype._neutrals.reon"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype._neutrals.</span>reon (spec, ms, host)](#apidoc.element.swarm.Host.prototype._neutrals.reon)
- description and source-code
```javascript
function hostReOn(spec, ms, host) {
    if (spec.type() !== 'Host') {
        throw new Error('Host.reon(/NotHost.reon)');
    }
    this.clock.adjustTime(ms);
    this.addSource(spec, host);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Host.prototype._ops"></a>[module swarm.Host.prototype._ops](#apidoc.module.swarm.Host.prototype._ops)

#### <a name="apidoc.element.swarm.Host.prototype._ops.init"></a>[function <span class="apidocSignatureSpan">swarm.Host.prototype._ops.</span>init (spec, state, src)](#apidoc.element.swarm.Host.prototype._ops.init)
- description and source-code
```javascript
init = function (spec, state, src) {

    var tail = {}, // ops to be applied on top of the received state
        typeid = spec.filter('/#'),
        lstn = this._lstn,
        a_spec;
    this._lstn = []; // prevent events from being fired

    if (state._version/* && state._version !== '!0'*/) {
        // local changes may need to be merged into the received state
        if (this._oplog) {
            for (a_spec in this._oplog) {
                tail[a_spec] = this._oplog[a_spec];
            }
            this._oplog = {};
        }
        this._vector && (this._vector = undefined);
        // zero everything
        for (var key in this) {
            if (this.hasOwnProperty(key) && key.charAt(0) !== '_') {
                this[key] = undefined;
            }
        }
        // set default values
        this.reset();

        this.apply(state);
        this._version = state._version;

        state._oplog && (this._oplog = state._oplog); // FIXME copy
        state._vector && (this._vector = state._vector);
    }
    // add the received tail to the local one
    if (state._tail) {
        for (a_spec in state._tail) {
            tail[a_spec] = state._tail[a_spec];
        }
    }
    // appply the combined tail to the new state
    var specs = [];
    for (a_spec in tail) {
        specs.push(a_spec);
    }
    specs.sort().reverse();
    // there will be some replays, but those will be ignored
    while (a_spec = specs.pop()) {
        this.deliver(typeid.add(a_spec), tail[a_spec], this);
    }

    this._lstn = lstn;

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.LamportClock"></a>[module swarm.LamportClock](#apidoc.module.swarm.LamportClock)

#### <a name="apidoc.element.swarm.LamportClock.LamportClock"></a>[function <span class="apidocSignatureSpan">swarm.</span>LamportClock (processId, initTime)](#apidoc.element.swarm.LamportClock.LamportClock)
- description and source-code
```javascript
LamportClock = function (processId, initTime) {
    if (!Spec.reTok.test(processId)) {
        throw new Error('invalid process id: '+processId);
    }
    this.id = processId;
    // sometimes we assume our local clock has some offset
    this.seq = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.LamportClock.prototype"></a>[module swarm.LamportClock.prototype](#apidoc.module.swarm.LamportClock.prototype)

#### <a name="apidoc.element.swarm.LamportClock.prototype.adjustTime"></a>[function <span class="apidocSignatureSpan">swarm.LamportClock.prototype.</span>adjustTime ()](#apidoc.element.swarm.LamportClock.prototype.adjustTime)
- description and source-code
```javascript
adjustTime = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LamportClock.prototype.checkTimestamp"></a>[function <span class="apidocSignatureSpan">swarm.LamportClock.prototype.</span>checkTimestamp (ts)](#apidoc.element.swarm.LamportClock.prototype.checkTimestamp)
- description and source-code
```javascript
function see(ts) {
    var parsed = this.parseTimestamp(ts);
    if (parsed.seq >= this.seq) {
        this.seq = parsed.seq + 1;
    }
    return true;
}
```
- example usage
```shell
...
                        seqi = 1; // FIXME repeat ids, double insert
                    }
                }
            }
        }
    }
    if (genTs) {
        this._host.clock.checkTimestamp(genTs);
    }
    this.weave = w1.join('');
    this.ids = w4;
    this.rebuild();
},
remove: function (spec, rm, src) {
    var w1 = [], w4 = [];
...
```

#### <a name="apidoc.element.swarm.LamportClock.prototype.issueTimestamp"></a>[function <span class="apidocSignatureSpan">swarm.LamportClock.prototype.</span>issueTimestamp ()](#apidoc.element.swarm.LamportClock.prototype.issueTimestamp)
- description and source-code
```javascript
function time() {
    var base = Spec.int2base(this.seq++, 5);
    return base + '+' + this.id;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LamportClock.prototype.parseTimestamp"></a>[function <span class="apidocSignatureSpan">swarm.LamportClock.prototype.</span>parseTimestamp (ts)](#apidoc.element.swarm.LamportClock.prototype.parseTimestamp)
- description and source-code
```javascript
function parse(ts) {
    var m = ts.match(Spec.reTokExt);
    if (!m) {throw new Error('malformed timestamp: '+ts);}
    return {
        seq: Spec.base2int(m[1]),
        process: m[2]
    };
}
```
- example usage
```shell
...
        seq: Spec.base2int(m[1]),
        process: m[2]
    };
};

/** Lamport partial order  imperfect semi-logical*/
LamportClock.prototype.checkTimestamp = function see (ts) {
    var parsed = this.parseTimestamp(ts);
    if (parsed.seq >= this.seq) {
        this.seq = parsed.seq + 1;
    }
    return true;
};

LamportClock.prototype.time2date = function () {
...
```

#### <a name="apidoc.element.swarm.LamportClock.prototype.time2date"></a>[function <span class="apidocSignatureSpan">swarm.LamportClock.prototype.</span>time2date ()](#apidoc.element.swarm.LamportClock.prototype.time2date)
- description and source-code
```javascript
time2date = function () {
    return undefined;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.LevelStorage"></a>[module swarm.LevelStorage](#apidoc.module.swarm.LevelStorage)

#### <a name="apidoc.element.swarm.LevelStorage.LevelStorage"></a>[function <span class="apidocSignatureSpan">swarm.</span>LevelStorage (id, options, callback)](#apidoc.element.swarm.LevelStorage.LevelStorage)
- description and source-code
```javascript
function LevelStorage(id, options, callback) {
    Storage.call(this);
    this.options = options;
    this._host = null; // will be set by the Host
    this.db = options.db;
    this._id = id;
    this.filename = null;
    if (this.db.constructor===Function) {
        this.db = this.db(options.path||id);
    }
    this.logtails = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.LevelStorage.prototype"></a>[module swarm.LevelStorage.prototype](#apidoc.module.swarm.LevelStorage.prototype)

#### <a name="apidoc.element.swarm.LevelStorage.prototype.close"></a>[function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>close (callback, error)](#apidoc.element.swarm.LevelStorage.prototype.close)
- description and source-code
```javascript
close = function (callback, error) { // FIXME
    if (error) {
        console.log("fatal IO error", error);
    }
    if (this.db) {
        this.db.close(callback);
        this.db = null;
    } else {
        callback(); // closed already
    }
}
```
- example usage
```shell
...
        }
    }, 1);
};

AsyncLoopbackConnection.prototype.close = function () {
    delete AsyncLoopbackConnection.pipes[this.id];
    var pair = this.pair();
    pair && pair.close();
    this.lstn.close && this.lstn.close();
};
...
```

#### <a name="apidoc.element.swarm.LevelStorage.prototype.off"></a>[function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>off (spec, val, src)](#apidoc.element.swarm.LevelStorage.prototype.off)
- description and source-code
```javascript
off = function (spec, val, src) {
    var ti = spec.filter('/#');
    delete this.logtails[ti];
    Storage.prototype.off.call(this,spec,val,src);
}
```
- example usage
```shell
...

/**
 * Unsubscribe from collections entries' events
 * @param {function(*)} callback
 * @this Set|Vector
 */
offObjectEvent: function (callback) {
    this._proxy.off(callback);
},

/**
 * Waits for collection to receive state from cache or uplink and then invokes passed callback
 *
 * @param {function()} callback
 * @this Set|Vector
...
```

#### <a name="apidoc.element.swarm.LevelStorage.prototype.open"></a>[function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>open (callback)](#apidoc.element.swarm.LevelStorage.prototype.open)
- description and source-code
```javascript
open = function (callback) {
    this.db.open(this.options.dbOptions||{}, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LevelStorage.prototype.readOps"></a>[function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>readOps (ti, callback)](#apidoc.element.swarm.LevelStorage.prototype.readOps)
- description and source-code
```javascript
readOps = function (ti, callback) {
    var self = this;
    var tail = {}, log = [];
    var i = this.db.iterator({
        gt: ti+' ',
        lt: ti+'0'
    });
    i.next(function recv(err,key,value){
        if (err) {
            callback(err);
            i.end(function(err){});
        } else if (key) {
            var spec = new Spec(key);
            var vo = spec.filter('!.');
            tail[vo] = JSON.parse(value.toString());
            log.push(vo);
            i.next(recv);
        } else {
            console.log('<TAIL',self._host && self._host._id,tail);
            self.logtails[ti] = ti in self.logtails ?
                self.logtails[ti].concat(log) : log;
            callback(null, tail);
            i.end(function(err){
                err && console.error("can't close an iter",err);
            });
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LevelStorage.prototype.readState"></a>[function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>readState (ti, callback)](#apidoc.element.swarm.LevelStorage.prototype.readState)
- description and source-code
```javascript
readState = function (ti, callback) {
    var self = this;
    ti = ti.toString();
    this.db.get(ti, {asBuffer:false}, function(err,value){

        var notFound = err && /^NotFound/.test(err.message);
        if (err && !notFound) { return callback(err); }

        if ((err && notFound) || !value) {
            err = null;
            value = {_version: '!0'};
        } else {
            value = JSON.parse(value);
        }

        console.log('<STATE',self._host && self._host._id,value);
        callback(err, value);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LevelStorage.prototype.writeOp"></a>[function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>writeOp (spec, value, cb)](#apidoc.element.swarm.LevelStorage.prototype.writeOp)
- description and source-code
```javascript
writeOp = function (spec, value, cb) {
    var json = JSON.stringify(value);
    var ti = spec.filter('/#');
    if (!this.logtails[ti]) {
        this.logtails[ti] = [];
    }
    this.logtails[ti].push(spec);
    console.log('>OP',spec.toString(),json);
    this.db.put(spec.toString(), json, function (err){
        err && console.error('op write error',err);
        cb(err);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LevelStorage.prototype.writeState"></a>[function <span class="apidocSignatureSpan">swarm.LevelStorage.prototype.</span>writeState (spec, state, cb)](#apidoc.element.swarm.LevelStorage.prototype.writeState)
- description and source-code
```javascript
writeState = function (spec, state, cb) {
    console.log('>STATE',state);
    var self = this;
    var ti = spec.filter('/#');
    //var save = JSON.stringify(state, undefined, 2);
    if (!self.db) {
        console.warn('the storage is not open', this._host&&this._host._id);
        return;
    }

    var json = JSON.stringify(state);
    var cleanup = [], key;
    if (ti in this.logtails) {
        while (key = this.logtails[ti].pop()) {
            cleanup.push({
                key: key,
                type: 'del'
            });
        }
        delete this.logtails[ti];
    }
    console.log('>FLUSH',json,cleanup.length);
    self.db.put(ti, json, function onSave(err) {
        if (!err && cleanup.length && self.db) {
            console.log('>CLEAN',cleanup);
            self.db.batch(cleanup, function(err){
                err && console.error('log trimming failed',err);
            });
        }
        err && console.error("state write error", err);
        cb(err);
    });

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.LongSpec"></a>[module swarm.LongSpec](#apidoc.module.swarm.LongSpec)

#### <a name="apidoc.element.swarm.LongSpec.LongSpec"></a>[function <span class="apidocSignatureSpan">swarm.</span>LongSpec (spec, codeBook)](#apidoc.element.swarm.LongSpec.LongSpec)
- description and source-code
```javascript
LongSpec = function (spec, codeBook) {
    var cb = this.codeBook = codeBook || {en:{},de:{}};
    if (!cb.en) { cb.en = {}; }
    if (!cb.de) { // revert en to make de
        cb.de = {};
        for(var tok in cb.en) {
            cb.de[cb.en[tok]] = tok;
        }
    }
    if (!cb.lastCodes) {
        cb.lastCodes = {'/':0x30,'#':0x30,'!':0x30,'.':0x30,'+':0x30};
    }
    // For a larger document, a single LongSpec may be some megabytes long.
    // As we don't want to rewrite those megabytes on every keypress, we
    // divide data into chunks.
    this.chunks = [];
    this.chunkLengths = [];
    if (spec) {
        this.append(spec);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.Iterator"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.</span>Iterator (owner, index)](#apidoc.element.swarm.LongSpec.Iterator)
- description and source-code
```javascript
function Iterator(owner, index) {
    this.owner = owner;         // our LongSpec
<span class="apidocCodeCommentSpan">    /*this.chunk = 0;             // the chunk we are in
    this.index = -1;            // token index (position "before the 1st token")
    this.chunkIndex = -1;       // token index within the chunk
    this.prevFull = undefined;  // previous full (non-collapsed) token
    //  seqStart IS the previous match or prev match is trivial
    this.prevCollapsed = 0;
    this.match = null;
    //this.next();*/
</span>    this.skip2chunk(0);
    if (index) {
        if (index.constructor===LongSpec.Iterator) {
            index = index.index;
        }
        this.skip(index);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.int2uni"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.</span>int2uni (i)](#apidoc.element.swarm.LongSpec.int2uni)
- description and source-code
```javascript
int2uni = function (i) {
    if (i<0 || i>0x7fffffff) { throw new Error('int is out of range'); }
    return String.fromCharCode( 0x30+(i>>15), 0x30+(i&0x7fff) );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.uni2int"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.</span>uni2int (uni)](#apidoc.element.swarm.LongSpec.uni2int)
- description and source-code
```javascript
uni2int = function (uni) {
    if (!/^[0-\u802f]{2}$/.test(uni)) {
        throw new Error('invalid unicode number') ;
    }
    return ((uni.charCodeAt(0)-0x30)<<15) | (uni.charCodeAt(1)-0x30);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.LongSpec.Iterator"></a>[module swarm.LongSpec.Iterator](#apidoc.module.swarm.LongSpec.Iterator)

#### <a name="apidoc.element.swarm.LongSpec.Iterator.Iterator"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.</span>Iterator (owner, index)](#apidoc.element.swarm.LongSpec.Iterator.Iterator)
- description and source-code
```javascript
function Iterator(owner, index) {
    this.owner = owner;         // our LongSpec
<span class="apidocCodeCommentSpan">    /*this.chunk = 0;             // the chunk we are in
    this.index = -1;            // token index (position "before the 1st token")
    this.chunkIndex = -1;       // token index within the chunk
    this.prevFull = undefined;  // previous full (non-collapsed) token
    //  seqStart IS the previous match or prev match is trivial
    this.prevCollapsed = 0;
    this.match = null;
    //this.next();*/
</span>    this.skip2chunk(0);
    if (index) {
        if (index.constructor===LongSpec.Iterator) {
            index = index.index;
        }
        this.skip(index);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.LongSpec.Iterator.prototype"></a>[module swarm.LongSpec.Iterator.prototype](#apidoc.module.swarm.LongSpec.Iterator.prototype)

#### <a name="apidoc.element.swarm.LongSpec.Iterator.prototype.clone"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>clone ()](#apidoc.element.swarm.LongSpec.Iterator.prototype.clone)
- description and source-code
```javascript
clone = function () {
    var copy = new LongSpec.Iterator(this.owner);
    copy.chunk = this.chunk;
    copy.match = this.match;
    copy.index = this.index;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.Iterator.prototype.decode"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>decode ()](#apidoc.element.swarm.LongSpec.Iterator.prototype.decode)
- description and source-code
```javascript
function decode() {
    if (this.match===null) { return undefined; }
    var quant = this.match[1];
    var body = this.match[3];
    var ext = this.match[4];
    var pm=this.prevFull, prevTok, prevQuant, prevBody, prevExt;
    var int1, int2, base1, base2;
    var de = quant;
    if (pm) {
        prevTok=pm[0], prevQuant=pm[1], prevBody=pm[3], prevExt=pm[4];
    }
    if (!body) {
        if (prevBody.length===1) {
            body = prevBody;
        } else {
            var l_1 = prevBody.length-1;
            var int = prevBody.charCodeAt(l_1);
            body = prevBody.substr(0,l_1) + String.fromCharCode(int+this.prevCollapsed+1);
        }
        ext = prevExt;
    }
    switch (body.length) {
        case 1:
            de += this.owner.codeBook.de[quant+body].substr(1); // TODO sep codebooks
            break;
        case 2:
            int1 = LongSpec.uni2int(body);
            base1 = Spec.int2base(int1,5);
            de += base1;
            break;
        case 3:
            int1 = LongSpec.uni2int(body.substr(0,2));
            int2 = LongSpec.uni2int('0'+body.charAt(2));
            base1 = Spec.int2base(int1,5);
            base2 = Spec.int2base(int2,2);
            de += base1 + base2;
            break;
        case 4:
            int1 = LongSpec.uni2int(body.substr(0,2));
            int2 = LongSpec.uni2int(body.substr(2,2));
            base1 = Spec.int2base(int1,5);
            base2 = Spec.int2base(int2,5);
            de += base1 + base2;
            break;
        default:
            de += body;
            break;
    }
    if (ext) {
        var deExt = this.owner.codeBook.de['+'+ext];
        de += deExt;
    }
    return de;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.Iterator.prototype.encode"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>encode (de)](#apidoc.element.swarm.LongSpec.Iterator.prototype.encode)
- description and source-code
```javascript
function encode(de) {
    var re = Spec.reQTokExt;
    re.lastIndex = 0;
    var m=re.exec(de); // this one is de
    if (!m || m[0].length!==de.length) {throw new Error('malformed token: '+de);}
    var tok=m[0], quant=m[1], body=m[3], ext=m[4];
    var pm = this.prevFull; // this one is en
    var prevTok, prevQuant, prevBody, prevExt;
    var enBody, enExt;
    if (pm) {
        prevTok=pm[0], prevQuant=pm[1], prevBody=pm[3], prevExt=pm[4]?'+'+pm[4]:undefined;
    }
    if (ext) {
        enExt = this.owner.codeBook.en['+'+ext] || this.owner.allocateCode('+'+ext);
    }
    var maySeq = pm && quant===prevQuant && enExt===prevExt;
    var haveSeq=false, seqBody = '';
    var int1, int2, uni1, uni2;
    //var expected = head + (counter===-1?'':Spec.int2base(counter+inc,1)) + tail;
    if ( body.length<=4 ||          // TODO make it a switch
         (quant in LongSpec.quants2code) ||
         (tok in this.owner.codeBook.en) ) {  // 1 symbol by the codebook

        enBody = this.owner.codeBook.en[quant+body] ||
                 this.owner.allocateCode(quant+body);
        enBody = enBody.substr(1); // FIXME separate codebooks 4 quants
        if (maySeq) {// seq coding for dictionary-coded
            seqBody = enBody;
        }
    } else if (body.length===5) { // 2-symbol base-2^15
        var int = Spec.base2int(body);
        enBody = LongSpec.int2uni(int);
        if (maySeq && prevBody.length===2) {
            seqBody = LongSpec.int2uni(int-this.prevCollapsed-1);
        }
    } else if (body.length===7) { // 3-symbol base-2^15
        int1 = Spec.base2int(body.substr(0,5));
        int2 = Spec.base2int(body.substr(5,2));
        uni1 = LongSpec.int2uni(int1);
        uni2 = LongSpec.int2uni(int2).charAt(1);
        enBody = uni1 + uni2;
        if (maySeq && prevBody.length===3) {
            seqBody = uni1 + LongSpec.int2uni(int2-this.prevCollapsed-1).charAt(1);
        }
    } else if (body.length===10) { // 4-symbol 60-bit long number
        int1 = Spec.base2int(body.substr(0,5));
        int2 = Spec.base2int(body.substr(5,5));
        uni1 = LongSpec.int2uni(int1);
        uni2 = LongSpec.int2uni(int2);
        enBody = uni1 + uni2;
        if (maySeq && prevBody.length===4) {
            seqBody = uni1+LongSpec.int2uni(int2-this.prevCollapsed-1);
        }
    } else { // verbatim
        enBody = body;
        seqBody = enBody;
    }
    haveSeq = seqBody===prevBody;
    return haveSeq ? quant : quant+enBody+(enExt||'');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.Iterator.prototype.end"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>end ()](#apidoc.element.swarm.LongSpec.Iterator.prototype.end)
- description and source-code
```javascript
end = function () {
    return this.match===null && this.chunk===this.owner.chunks.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.Iterator.prototype.erase"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>erase (count)](#apidoc.element.swarm.LongSpec.Iterator.prototype.erase)
- description and source-code
```javascript
erase = function (count) {
    if (this.end()) {return;}
    count = count || 1;
    var chunks = this.owner.chunks;
    var lengths = this.owner.chunkLengths;
    // remember offsets
    var fromChunk = this.chunk;
    var fromOffset = this.match.index;
    var fromChunkIndex = this.chunkIndex; // TODO clone USE 2 iterators or i+c

    count = this.skip(count); // checked for runaway skip()
    // the iterator now is at the first-after-erased pos

    var tillChunk = this.chunk;
    var tillOffset = this.match ? this.match.index : 0; // end()

    var collapsed = this.match && this.match[0].length===1;

    // splice strings, adjust indexes
    if (fromChunk===tillChunk) {
        var chunk = chunks[this.chunk];
        var pre = chunk.substr(0,fromOffset);
        var post = chunk.substr(tillOffset);
        if (collapsed) { // sequence is broken now; needs expansion
            post = this.token() + post.substr(1);
        }
        chunks[this.chunk] = pre + post;
        lengths[this.chunk] -= count;
        this.chunkIndex -= count;
    } else {  // FIXME refac, more tests (+wear)
        if (fromOffset===0) {
            fromChunk--;
        } else {
            chunks[fromChunk] = chunks[fromChunk].substr(0,fromOffset);
            lengths[fromChunk] = fromChunkIndex;
        }
        var midChunks = tillChunk - fromChunk - 1;
        if (midChunks) { // wipe'em out
            //for(var c=fromChunk+1; c<tillChunk; c++) ;
            chunks.splice(fromChunk+1,midChunks);
            lengths.splice(fromChunk+1,midChunks);
        }
        if (tillChunk<chunks.length && tillOffset>0) {
            chunks[tillChunk] = chunks[tillChunk].substr(this.match.index);
            lengths[tillChunk] -= this.chunkIndex;
            this.chunkIndex = 0;
        }
    }
    this.index -= count;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.Iterator.prototype.insert"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>insert (de)](#apidoc.element.swarm.LongSpec.Iterator.prototype.insert)
- description and source-code
```javascript
insert = function (de) { // insertBefore

    var insStr = this.encode(de);

    var brokenSeq = this.match && this.match[0].length===1;

    var re = LongSpec.Iterator.reTok;
    var chunks = this.owner.chunks, lengths = this.owner.chunkLengths;
    if (this.chunk==chunks.length) { // end(), append
        if (chunks.length>0) {
            var ind = this.chunk - 1;
            chunks[ind] += insStr;
            lengths[ind] ++;
        } else {
            chunks.push(insStr);
            lengths.push(1);
            this.chunk++;
        }
    } else {
        var chunkStr = chunks[this.chunk];
        var preEq = chunkStr.substr(0, this.match.index);
        var postEq = chunkStr.substr(this.match.index);
        if (brokenSeq) {
            var me = this.token();
            this.prevFull = undefined;
            var en = this.encode(me);
            chunks[this.chunk] = preEq + insStr + en + postEq.substr(1);
            re.lastIndex = preEq.length + insStr.length;
            this.match = re.exec(chunks[this.chunk]);
        } else {
            chunks[this.chunk] = preEq + insStr + /**/ postEq;
            this.match.index += insStr.length;
        }
        lengths[this.chunk] ++;
        this.chunkIndex ++;
    }
    this.index ++;
    if (insStr.length>1) {
        re.lastIndex = 0;
        this.prevFull = re.exec(insStr);
        this.prevCollapsed = 0;
    } else {
        this.prevCollapsed++;
    }

    // may split chunks
    // may join chunks
}
```
- example usage
```shell
...
            }
            break;
        case '=':
            skip(val.length);
        }
    }
    rm && this.remove(rm);
    ins && this.insert(ins);
}
});

Text.diff = function diff(was, is) {
var ret = [];
// prefix suffix the rest is change
var pre = 0;
...
```

#### <a name="apidoc.element.swarm.LongSpec.Iterator.prototype.insertBlock"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>insertBlock (de)](#apidoc.element.swarm.LongSpec.Iterator.prototype.insertBlock)
- description and source-code
```javascript
insertBlock = function (de) { // insertBefore
    var re = Spec.reQTokExt;
    var toks = de.match(re).reverse(), tok;
    while (tok=toks.pop()) {
        this.insert(tok);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.Iterator.prototype.next"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>next ( )](#apidoc.element.swarm.LongSpec.Iterator.prototype.next)
- description and source-code
```javascript
next = function ( ) {

    if (this.end()) {return;}

    var re = LongSpec.Iterator.reTok;
    re.lastIndex = this.match ? this.match.index+this.match[0].length : 0;
    var chunk = this.owner.chunks[this.chunk];

    if (chunk.length===re.lastIndex) {
        this.chunk++;
        this.chunkIndex = 0;
        if (this.match && this.match[0].length>0) {
            this.prevFull = this.match;
            this.prevCollapsed = 0;
        } else if (this.match) {
            this.prevCollapsed++;
        } else { // empty
            this.prevFull = undefined;
            this.prevCollapsed = 0;
        }
        this.match = null;
        this.index ++;
        if (this.end()) {return;}
    }

    if (this.match[0].length>1) {
        this.prevFull = this.match;
        this.prevCollapsed = 0;
    } else {
        this.prevCollapsed++;
    }

    this.match = re.exec(chunk);
    this.index++;
    this.chunkIndex++;

    return this.match[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.Iterator.prototype.skip"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>skip ( count )](#apidoc.element.swarm.LongSpec.Iterator.prototype.skip)
- description and source-code
```javascript
skip = function ( count ) {
    // TODO may implement fast-skip of seq-compressed spans
    var lengths = this.owner.chunkLengths, chunks = this.owner.chunks;
    count = count || 1;
    var left = count;
    var leftInChunk = lengths[this.chunk]-this.chunkIndex;
    if ( leftInChunk <= count ) { // skip chunks
        left -= leftInChunk; // skip the current chunk
        var c=this.chunk+1;    // how many extra chunks to skip
        while (left>chunks[c] && c<chunks.length) {
            left-=chunks[++c];
        }
        this.skip2chunk(c);
    }
    if (this.chunk<chunks.length) {
        while (left>0) {
            this.next();
            left--;
        }
    }
    return count - left;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.Iterator.prototype.skip2chunk"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>skip2chunk ( chunk )](#apidoc.element.swarm.LongSpec.Iterator.prototype.skip2chunk)
- description and source-code
```javascript
skip2chunk = function ( chunk ) {
    var chunks = this.owner.chunks;
    if (chunk===undefined) {chunk=chunks.length;}
    this.index = 0;
    for(var c=0; c<chunk; c++) { // TODO perf pick the current value
        this.index += this.owner.chunkLengths[c];
    }
    this.chunkIndex = 0;
    this.chunk = chunk;
    var re = LongSpec.Iterator.reTok;
    if ( chunk < chunks.length ) {
        re.lastIndex = 0;
        this.match = re.exec(chunks[this.chunk]);
    } else {
        this.match = null;
    }
    if (chunk>0) { // (1) chunks must not be empty; (2) a chunk starts with a full token
        var prev = chunks[chunk-1];
        var j = 0;
        while (Spec.quants.indexOf(prev.charAt(prev.length-1-j)) !== -1) { j++; }
        this.prevCollapsed = j;
        var k = 0;
        while (Spec.quants.indexOf(prev.charAt(prev.length-1-j-k))===-1) { k++; }
        re.lastIndex = prev.length-1-j-k;
        this.prevFull = re.exec(prev);
    } else {
        this.prevFull = undefined;
        this.prevCollapsed = 0;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.Iterator.prototype.token"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.Iterator.prototype.</span>token ()](#apidoc.element.swarm.LongSpec.Iterator.prototype.token)
- description and source-code
```javascript
token = function () {
    return this.decode();
}
```
- example usage
```shell
...
    state: function (spec, text, src) {
        console.log('what?');
    }
},
ops: {
    insert: function (spec, ins, src) {
        var w1 = [], w4 = [];
        var vt = spec.token('!'), v = vt.bare;
        var ts = v.substr(0, 5), seq = v.substr(5) || '00';
        var seqi = Spec.base2int(seq);
        for (var i = 0; i < this.weave.length; i++) {
            var id = this.ids[i];
            w1.push(this.weave.charAt(i));
            w4.push(id);
            if (id in ins) {
...
```



# <a name="apidoc.module.swarm.LongSpec.prototype"></a>[module swarm.LongSpec.prototype](#apidoc.module.swarm.LongSpec.prototype)

#### <a name="apidoc.element.swarm.LongSpec.prototype.add"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>add (spec)](#apidoc.element.swarm.LongSpec.prototype.add)
- description and source-code
```javascript
function ls_add(spec) {
    var pos = this.end();
    pos.insertBlock(spec);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.prototype.allocateCode"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>allocateCode (tok)](#apidoc.element.swarm.LongSpec.prototype.allocateCode)
- description and source-code
```javascript
allocateCode = function (tok) {
    var quant = tok.charAt(0);
    //if (Spec.quants.indexOf(quant)===-1) {throw new Error('invalid token');}
    var en, cb = this.codeBook, lc = cb.lastCodes;
    if (lc[quant]<'z'.charCodeAt(0)) { // pick a nice letter
        for(var i=1; !en && i<tok.length; i++) {
            var x = tok.charAt(i), e = quant+x;
            if (!cb.de[e]) {  en = e;  }
        }
    }
    while (!en && lc[quant]<0x802f) {
        var y = String.fromCharCode(lc[quant]++);
        var mayUse = quant + y;
        if ( ! cb.en[mayUse] ) {  en = mayUse;  }
    }
    if (!en) {
        if (tok.length<=3) {
            throw new Error("out of codes");
        }
        en = tok;
    }
    cb.en[tok] = en;
    cb.de[en] = tok;
    return en;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.prototype.append"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>append (spec)](#apidoc.element.swarm.LongSpec.prototype.append)
- description and source-code
```javascript
function ls_add(spec) {
    var pos = this.end();
    pos.insertBlock(spec);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.prototype.charLength"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>charLength ()](#apidoc.element.swarm.LongSpec.prototype.charLength)
- description and source-code
```javascript
charLength = function () {
    var len = 0;
    for(var i=0; i<this.chunks.length; i++) {
        len += this.chunks[i].length;
    }
    return len;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.prototype.end"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>end ()](#apidoc.element.swarm.LongSpec.prototype.end)
- description and source-code
```javascript
end = function () {
    var e = new LongSpec.Iterator(this);
    e.skip2chunk(this.chunks.length);
    return e;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.prototype.find"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>find (tok, startIndex)](#apidoc.element.swarm.LongSpec.prototype.find)
- description and source-code
```javascript
find = function (tok, startIndex) {
    //var en = this.encode(tok).toString(); // don't split on +
    var i = this.iterator(startIndex);
    while (!i.end()) {
        if (i.token()===tok) {
            return i;
        }
        i.next();
    }
    return i;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>indexOf (tok, startAt)](#apidoc.element.swarm.LongSpec.prototype.indexOf)
- description and source-code
```javascript
indexOf = function (tok, startAt) {
    var iter = this.find(tok,startAt);
    return iter.end() ? -1 : iter.index;
}
```
- example usage
```shell
...
ProxyListener.prototype.on = function (callback) {
    if (this.callbacks===null) { this.callbacks = []; }
    this.callbacks.push(callback);
};

ProxyListener.prototype.off = function (callback) {
    if (this.callbacks===null) { return; }
    var i = this.callbacks.indexOf(callback);
    if (i!==-1) {
        this.callbacks.splice(i,1);
    } else {
        console.warn('listener unknown', callback);
    }
};
...
```

#### <a name="apidoc.element.swarm.LongSpec.prototype.insert"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>insert (tok, i)](#apidoc.element.swarm.LongSpec.prototype.insert)
- description and source-code
```javascript
insert = function (tok, i) {
    var iter = i.constructor===LongSpec.Iterator ? i : this.iterator(i);
    iter.insertBlock(tok);
}
```
- example usage
```shell
...
            }
            break;
        case '=':
            skip(val.length);
        }
    }
    rm && this.remove(rm);
    ins && this.insert(ins);
}
});

Text.diff = function diff(was, is) {
var ret = [];
// prefix suffix the rest is change
var pre = 0;
...
```

#### <a name="apidoc.element.swarm.LongSpec.prototype.iterator"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>iterator (index)](#apidoc.element.swarm.LongSpec.prototype.iterator)
- description and source-code
```javascript
iterator = function (index) {
    return new LongSpec.Iterator(this,index);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.prototype.length"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>length ()](#apidoc.element.swarm.LongSpec.prototype.length)
- description and source-code
```javascript
length = function () { // TODO .length ?
    var len = 0;
    for(var i=0; i<this.chunks.length; i++) {
        len += this.chunkLengths[i];
    }
    return len;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.LongSpec.prototype.toString"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>toString ()](#apidoc.element.swarm.LongSpec.prototype.toString)
- description and source-code
```javascript
toString = function () {
    var ret = [];
    for(var i = this.iterator(); !i.end(); i.next()){
        ret.push(i.decode());
    }
    return ret.join('');
}
```
- example usage
```shell
...

AsyncLoopbackConnection.prototype.receive = function (string) {
this.lstn.data && this.lstn.data(string);
};

AsyncLoopbackConnection.prototype.write = function (obj) {
var self = this;
obj && self.queue.push(obj.toString());
setTimeout(function () {
    var pair = self.pair();
    if (!pair) {
        return;
    }
    while (self.queue.length) {
        pair.receive(self.queue.shift());
...
```

#### <a name="apidoc.element.swarm.LongSpec.prototype.tokenAt"></a>[function <span class="apidocSignatureSpan">swarm.LongSpec.prototype.</span>tokenAt (pos)](#apidoc.element.swarm.LongSpec.prototype.tokenAt)
- description and source-code
```javascript
tokenAt = function (pos) {
    var iter = this.iterator(pos);
    return iter.token();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.MinutePreciseClock"></a>[module swarm.MinutePreciseClock](#apidoc.module.swarm.MinutePreciseClock)

#### <a name="apidoc.element.swarm.MinutePreciseClock.MinutePreciseClock"></a>[function <span class="apidocSignatureSpan">swarm.</span>MinutePreciseClock (processId, timeOffsetMs)](#apidoc.element.swarm.MinutePreciseClock.MinutePreciseClock)
- description and source-code
```javascript
MinutePreciseClock = function (processId, timeOffsetMs) {
    if (!Spec.reTok.test(processId)) {
        throw new Error('invalid process id: '+processId);
    }
    this.id = processId;
    // sometimes we assume our local clock has some offset
    this.clockOffsetMs = 0;
    this.lastIssuedTimestamp = '';
    // although we try hard to use wall clock time, we must
    // obey Lamport logical clock rules, in particular our
    // timestamps must be greater than any other timestamps
    // previously seen
    this.lastTimeSeen = 0;
    this.lastSeqSeen = 0;
    if (timeOffsetMs) {
        this.clockOffsetMs = timeOffsetMs;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.MinutePreciseClock.prototype"></a>[module swarm.MinutePreciseClock.prototype](#apidoc.module.swarm.MinutePreciseClock.prototype)

#### <a name="apidoc.element.swarm.MinutePreciseClock.prototype.adjustTime"></a>[function <span class="apidocSignatureSpan">swarm.MinutePreciseClock.prototype.</span>adjustTime (trueMs)](#apidoc.element.swarm.MinutePreciseClock.prototype.adjustTime)
- description and source-code
```javascript
adjustTime = function (trueMs) {
    // TODO use min historical offset
    var localTime = new Date().getTime();
    var clockOffsetMs = trueMs - localTime;
    this.clockOffsetMs = clockOffsetMs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.MinutePreciseClock.prototype.checkTimestamp"></a>[function <span class="apidocSignatureSpan">swarm.MinutePreciseClock.prototype.</span>checkTimestamp (ts)](#apidoc.element.swarm.MinutePreciseClock.prototype.checkTimestamp)
- description and source-code
```javascript
function see(ts) {
    if (ts<this.lastIssuedTimestamp) { return true; }
    var parsed = this.parseTimestamp(ts);
    if (parsed.time<this.lastTimeSeen) { return true; }
    var min = this.minutes();
    if (parsed.time>min+1) { return false; } // bad clocks somewhere
    this.lastTimeSeen = parsed.time;
    this.lastSeqSeen = parsed.seq;
    return true;
}
```
- example usage
```shell
...
                        seqi = 1; // FIXME repeat ids, double insert
                    }
                }
            }
        }
    }
    if (genTs) {
        this._host.clock.checkTimestamp(genTs);
    }
    this.weave = w1.join('');
    this.ids = w4;
    this.rebuild();
},
remove: function (spec, rm, src) {
    var w1 = [], w4 = [];
...
```

#### <a name="apidoc.element.swarm.MinutePreciseClock.prototype.issueTimestamp"></a>[function <span class="apidocSignatureSpan">swarm.MinutePreciseClock.prototype.</span>issueTimestamp ()](#apidoc.element.swarm.MinutePreciseClock.prototype.issueTimestamp)
- description and source-code
```javascript
issueTimestamp = function () {
    var time = this.minutes();
    if (this.lastTimeSeen>time) { time = this.lastTimeSeen; }
    if (time>this.lastTimeSeen) { this.lastSeqSeen = -1; }
    this.lastTimeSeen = time;
    var seq = ++this.lastSeqSeen;
    if (seq>=(1<<18)) {throw new Error('max event freq is 4000Hz');}

    var baseTime = Spec.int2base(time, 4), baseSeq;
    if (seq<64) {
        baseSeq = Spec.int2base(seq, 1);
    } else {
        baseSeq = Spec.int2base(seq, 3);
    }

    this.lastIssuedTimestamp = baseTime + baseSeq + '+' + this.id;
    return this.lastIssuedTimestamp;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.MinutePreciseClock.prototype.minutes"></a>[function <span class="apidocSignatureSpan">swarm.MinutePreciseClock.prototype.</span>minutes ()](#apidoc.element.swarm.MinutePreciseClock.prototype.minutes)
- description and source-code
```javascript
minutes = function () {
    var millis = new Date().getTime();
    millis -= MinutePreciseClock.EPOCH;
    millis += this.clockOffsetMs;
    return (millis/60000) | 0;
}
```
- example usage
```shell
...
var millis = new Date().getTime();
millis -= MinutePreciseClock.EPOCH;
millis += this.clockOffsetMs;
return (millis/60000) | 0;
};

MinutePreciseClock.prototype.issueTimestamp = function () {
var time = this.minutes();
if (this.lastTimeSeen>time) { time = this.lastTimeSeen; }
if (time>this.lastTimeSeen) { this.lastSeqSeen = -1; }
this.lastTimeSeen = time;
var seq = ++this.lastSeqSeen;
if (seq>=(1<<18)) {throw new Error('max event freq is 4000Hz');}

var baseTime = Spec.int2base(time, 4), baseSeq;
...
```

#### <a name="apidoc.element.swarm.MinutePreciseClock.prototype.parseTimestamp"></a>[function <span class="apidocSignatureSpan">swarm.MinutePreciseClock.prototype.</span>parseTimestamp (ts)](#apidoc.element.swarm.MinutePreciseClock.prototype.parseTimestamp)
- description and source-code
```javascript
function parse(ts) {
    var m = ts.match(Spec.reTokExt);
    if (!m) {throw new Error('malformed timestamp: '+ts);}
    var timeseq=m[1]; //, process=m[2];
    var time = timeseq.substr(0,4), seq = timeseq.substr(4);
    if (seq.length!==1 && seq.length!==3) {
        throw new Error('malformed timestamp value: '+timeseq);
    }
    return {
        time: Spec.base2int(time),
        seq: Spec.base2int(seq)
    };
}
```
- example usage
```shell
...
        seq: Spec.base2int(m[1]),
        process: m[2]
    };
};

/** Lamport partial order  imperfect semi-logical*/
LamportClock.prototype.checkTimestamp = function see (ts) {
    var parsed = this.parseTimestamp(ts);
    if (parsed.seq >= this.seq) {
        this.seq = parsed.seq + 1;
    }
    return true;
};

LamportClock.prototype.time2date = function () {
...
```

#### <a name="apidoc.element.swarm.MinutePreciseClock.prototype.time2date"></a>[function <span class="apidocSignatureSpan">swarm.MinutePreciseClock.prototype.</span>time2date ()](#apidoc.element.swarm.MinutePreciseClock.prototype.time2date)
- description and source-code
```javascript
time2date = function () {
    // parse etc
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Model"></a>[module swarm.Model](#apidoc.module.swarm.Model)

#### <a name="apidoc.element.swarm.Model.Model"></a>[function <span class="apidocSignatureSpan">swarm.</span>Model (idOrState)](#apidoc.element.swarm.Model.Model)
- description and source-code
```javascript
function Model(idOrState) {
    var ret = Model._super.apply(this, arguments);
    /// TODO: combine with state push, make clean
    if (ret === this && idOrState && idOrState.constructor !== String && !Spec.is(idOrState)) {
        this.deliver(this.spec().add(this._id, '!').add('.set'), idOrState);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model._super"></a>[function <span class="apidocSignatureSpan">swarm.Model.</span>_super ()](#apidoc.element.swarm.Model._super)
- description and source-code
```javascript
function Syncable() {
    // listeners represented as objects that have deliver() method
    this._lstn = [',']; // we unshift() uplink listeners and push() downlinks
    // ...so _lstn is like [server1, server2, storage, ',', view, listener]
    // The most correct way to specify a version is the version vector,
    // but that one may consume more space than the data itself in some cases.
    // Hence, _version is not a fully specified version vector (see version()
    // instead). _version is essentially is the greatest operation timestamp
    // (Lamport-like, i.e. "time+source"), sometimes amended with additional
    // timestamps. Its main features:
    // (1) changes once the object's state changes
    // (2) does it monotonically (in the alphanum order sense)
    this._version = '';
    // make sense of arguments
    var args = Array.prototype.slice.call(arguments);
    this._host = (args.length && args[args.length - 1]._type === 'Host') ?
            args.pop() : env.localhost;
    if (Spec.is(args[0])) {
        this._id = new Spec(args.shift()).id() || this._host.time();
    } else if (typeof(args[0]) === 'string') {
        this._id = args.shift(); // TODO format
    } else {
        this._id = this._host.time();
        this._version = '!0'; // may apply state in the constructor, see Model
    }
    //var state = args.length ? args.pop() : (fresh?{}:undefined);
    // register with the host
    var doubl = this._host.register(this);
    if (doubl !== this) { return doubl; }
    // locally created objects get state immediately
    // (while external-id objects need to query uplinks)
<span class="apidocCodeCommentSpan">    /*if (fresh && state) {
     state._version = '!'+this._id;
     var pspec = this.spec().add(state._version).add('.init');
     this.deliver(pspec,state,this._host);
     }*/
</span>    this.reset();
    // find uplinks, subscribe
    this.checkUplink();
    // TODO inplement state push
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model.addReaction"></a>[function <span class="apidocSignatureSpan">swarm.Model.</span>addReaction (methodOrField, fn)](#apidoc.element.swarm.Model.addReaction)
- description and source-code
```javascript
addReaction = function (methodOrField, fn) {
    var proto = this.prototype;
    if (typeof (proto[methodOrField]) === 'function') { // it is a field name
        return Syncable.addReaction.call(this, methodOrField, fn);
    } else {
        var wrapper = function (spec, val) {
            if (methodOrField in val) {
                fn.apply(this, arguments);
            }
        };
        wrapper._rwrap = true;
        return Syncable.addReaction.call(this, 'set', wrapper);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model.extend"></a>[function <span class="apidocSignatureSpan">swarm.Model.</span>extend (fn, own)](#apidoc.element.swarm.Model.extend)
- description and source-code
```javascript
extend = function (fn, own) {
    var parent = this, fnid;
    if (fn.constructor !== Function) {
        var id = fn.toString();
        fn = function SomeSyncable() {
            return parent.apply(this, arguments);
        };
        fnid = id; // if only it worked
    } else { // please call Syncable.constructor.apply(this,args) in your constructor
        fnid = fnname(fn);
    }

    // inheritance trick from backbone.js
    var SyncProto = function () {
        this.constructor = fn;
        this._neutrals = {};
        this._ops = {};
        this._reactions = {};

        var event,
            name;
        if (parent._pt) {
            //copy _neutrals & _ops from parent
            for (event in parent._pt._neutrals) {
                this._neutrals[event] = parent._pt._neutrals[event];
            }
            for (event in parent._pt._ops) {
                this._ops[event] = parent._pt._ops[event];
            }
        }

        // "Methods" are serialized, logged and delivered to replicas
        for (name in own.ops || {}) {
            if (Syncable.reMethodName.test(name)) {
                this._ops[name] = own.ops[name];
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid op name:',name);
            }
        }

        // "Neutrals" don't change the state
        for (name in own.neutrals || {}) {
            if (Syncable.reMethodName.test(name)) {
                this._neutrals[name] = own.neutrals[name];
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid neutral op name:',name);
            }
        }

        // "Remotes" are serialized and sent upstream (like RPC calls)
        for (name in own.remotes || {}) {
            if (Syncable.reMethodName.test(name)) {
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid rpc name:',name);
            }
        }

        // add mixins
        (own.mixins || []).forEach(function (mixin) {
            for (var name in mixin) {
                this[name] = mixin[name];
            }
        }, this);

        // add other members
        for (name in own) {
            if (Syncable.reMethodName.test(name)) {
                var memberType = own[name].constructor;
                if (memberType === Function) { // non-op method
                    // these must change state ONLY by invoking ops
                    this[name] = own[name];
                } else if (memberType===String || memberType===Number) {
                    this[name] = own[name]; // some static constant, OK
                } else if (name in Syncable.memberClasses) {
                    // see above
                    continue;
                } else {
                    console.warn('invalid member:',name,memberType);
                }
            } else {
                console.warn('invalid member name:',name);
            }
        }

        // add reactions
        for (name in own.reactions || {}) {
            var reaction = own.reactions[name];
            if (!reaction) { continue; }

            switch (typeof reaction) {
            case 'function':
                // handler-function
                this._reactions[name] = [reaction];
                break;
            case 'string':
                // handler-method name
                this._reactions[name] = [this[name]];
                break;
            default:
                if (reaction.constructor === Array) {
                    // array of handlers
                    this._reactions[name] = reaction.map(function (item) {
                        switch (typeof item) {
                        case 'function':
                            return item;
                        case 'string':
                            return this[item];
                        default:
                            throw new Error('unexpected reaction type');
                        }
                    }, this);
                } else {
                    throw new Error('unex ...
```
- example usage
```shell
...
these demos are normally online at http://ppyr.us and http://ppyr.us:8001/demo3/index.html respectively.

### Creating your first simple synchronized type

'''js
var Swarm = require('swarm');

var Mouse = Swarm.Model.extend('Mouse', {
    defaults: {
        name: 'Mickey',
        x: 0,
        y: 0
    }
});
...
```

#### <a name="apidoc.element.swarm.Model.removeReaction"></a>[function <span class="apidocSignatureSpan">swarm.Model.</span>removeReaction (handle)](#apidoc.element.swarm.Model.removeReaction)
- description and source-code
```javascript
removeReaction = function (handle) {
    var op = handle.op,
        fn = handle.fn,
        list = this.prototype._reactions[op],
        i = list.indexOf(fn);
    if (i === -1) {
        throw new Error('reaction unknown');
    }
    list[i] = undefined; // such a peculiar pattern not to mess up out-of-callback removal
    while (list.length && !list[list.length - 1]) {
        list.pop();
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Model.prototype"></a>[module swarm.Model.prototype](#apidoc.module.swarm.Model.prototype)

#### <a name="apidoc.element.swarm.Model.prototype.callReactions"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>callReactions (spec, value, src)](#apidoc.element.swarm.Model.prototype.callReactions)
- description and source-code
```javascript
callReactions = function (spec, value, src) {
    var superReactions = syncProto._super.callReactions;
    if ('function' === typeof superReactions) {
        superReactions.call(this, spec, value, src);
    }
    var r = syncProto._reactions[spec.op()];
    if (r) {
        r.constructor !== Array && (r = [r]);
        for (var i = 0; i < r.length; i++) {
            r[i] && r[i].call(this, spec, value, src);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model.prototype.constructor"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>constructor (idOrState)](#apidoc.element.swarm.Model.prototype.constructor)
- description and source-code
```javascript
function Model(idOrState) {
    var ret = Model._super.apply(this, arguments);
    /// TODO: combine with state push, make clean
    if (ret === this && idOrState && idOrState.constructor !== String && !Spec.is(idOrState)) {
        this.deliver(this.spec().add(this._id, '!').add('.set'), idOrState);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model.prototype.distillLog"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>distillLog ()](#apidoc.element.swarm.Model.prototype.distillLog)
- description and source-code
```javascript
distillLog = function () {
    // explain
    var sets = [],
        cumul = {},
        heads = {},
        spec;
    for (var s in this._oplog) {
        spec = new Spec(s);
        //if (spec.op() === 'set') {
        sets.push(spec);
        //}
    }
    sets.sort();
    for (var i = sets.length - 1; i >= 0; i--) {
        spec = sets[i];
        var val = this._oplog[spec],
            notempty = false;
        for (var field in val) {
            if (field in cumul) {
                delete val[field];
            } else {
                notempty = cumul[field] = val[field]; //store last value of the field
            }
        }
        var source = spec.source();
        notempty || (heads[source] && delete this._oplog[spec]);
        heads[source] = true;
    }
    return cumul;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model.prototype.fill"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>fill (key)](#apidoc.element.swarm.Model.prototype.fill)
- description and source-code
```javascript
fill = function (key) { // TODO goes to Model to support references
    if (!this.hasOwnProperty(key)) {
        throw new Error('no such entry');
    }

    //if (!Spec.is(this[key]))
    //    throw new Error('not a specifier');
    var spec = new Spec(this[key]).filter('/#');
    if (spec.pattern() !== '/#') {
        throw new Error('incomplete spec');
    }

    this[key] = this._host.get(spec);
<span class="apidocCodeCommentSpan">    /* TODO new this.refType(id) || new Swarm.types[type](id);
     on('init', function(){
     self.emit('fill',key,this)
     self.emit('full',key,this)
     });*/
</span>}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model.prototype.off"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>off ()](#apidoc.element.swarm.Model.prototype.off)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
...

/**
 * Unsubscribe from collections entries' events
 * @param {function(*)} callback
 * @this Set|Vector
 */
offObjectEvent: function (callback) {
    this._proxy.off(callback);
},

/**
 * Waits for collection to receive state from cache or uplink and then invokes passed callback
 *
 * @param {function()} callback
 * @this Set|Vector
...
```

#### <a name="apidoc.element.swarm.Model.prototype.on"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>on ()](#apidoc.element.swarm.Model.prototype.on)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.Model.prototype.packState"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>packState (state)](#apidoc.element.swarm.Model.prototype.packState)
- description and source-code
```javascript
packState = function (state) {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model.prototype.save"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>save ()](#apidoc.element.swarm.Model.prototype.save)
- description and source-code
```javascript
save = function () {
    var cumul = this.distillLog(),
        changes = {},
        pojo = this.pojo(),
        field;
    for (field in pojo) {
        if (this[field] !== cumul[field]) {// TODO nesteds
            changes[field] = this[field];
        }
    }
    for (field in cumul) {
        if (!(field in pojo)) {
            changes[field] = null; // JSON has no undefined
        }
    }
    this.set(changes);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model.prototype.set"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>set ()](#apidoc.element.swarm.Model.prototype.set)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
...

// 3.a. create an object
var someMouse = new Mouse();
// OR swarmHost.get('/Mouse');
// OR new Mouse({x:1, y:2});

// 4.a. a locally created object may be touched immediately
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
...
```

#### <a name="apidoc.element.swarm.Model.prototype.unpackState"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>unpackState (state)](#apidoc.element.swarm.Model.prototype.unpackState)
- description and source-code
```javascript
unpackState = function (state) {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model.prototype.validate"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype.</span>validate (spec, val)](#apidoc.element.swarm.Model.prototype.validate)
- description and source-code
```javascript
validate = function (spec, val) {
    if (spec.op() !== 'set') {
        return '';
    } // no idea
    for (var key in val) {
        if (!Syncable.reFieldName.test(key)) {
            return 'bad field name';
        }
    }
    return '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Model.prototype._neutrals"></a>[module swarm.Model.prototype._neutrals](#apidoc.module.swarm.Model.prototype._neutrals)

#### <a name="apidoc.element.swarm.Model.prototype._neutrals.error"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype._neutrals.</span>error (spec, val, repl)](#apidoc.element.swarm.Model.prototype._neutrals.error)
- description and source-code
```javascript
error = function (spec, val, repl) {
    console.error('something failed:', spec, val, '@', (repl && repl._id));
}
```
- example usage
```shell
...
        this.buf = buf; //will wait for "open"
    }
    ws.on('close', function () { ln.close && ln.close(); });
    ws.on('data', function (msg) {
        try {
            ln.data && ln.data(msg);
        } catch (ex) {
            console.error('message processing fails', ex);
            ln.error && ln.error(ex.message);
        }
    });
}

module.exports = SockJSStream;
...
```

#### <a name="apidoc.element.swarm.Model.prototype._neutrals.off"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype._neutrals.</span>off (spec, base, repl)](#apidoc.element.swarm.Model.prototype._neutrals.off)
- description and source-code
```javascript
off = function (spec, base, repl) {
    var ls = this._lstn;
    if (typeof(repl) === 'function') { // TODO ugly
        for (var i = 0; i < ls.length; i++) {
            if (ls[i] && ls[i].fn === repl && ls[i].key === base) {
                repl = ls[i];
                break;
            }
        }
    }
    Syncable._pt._neutrals.off.apply(this, arguments);
}
```
- example usage
```shell
...

/**
 * Unsubscribe from collections entries' events
 * @param {function(*)} callback
 * @this Set|Vector
 */
offObjectEvent: function (callback) {
    this._proxy.off(callback);
},

/**
 * Waits for collection to receive state from cache or uplink and then invokes passed callback
 *
 * @param {function()} callback
 * @this Set|Vector
...
```

#### <a name="apidoc.element.swarm.Model.prototype._neutrals.on"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype._neutrals.</span>on (spec, base, repl)](#apidoc.element.swarm.Model.prototype._neutrals.on)
- description and source-code
```javascript
on = function (spec, base, repl) {
    //  support the model.on('field',callback_fn) pattern
    if (typeof(repl) === 'function' &&
            typeof(base) === 'string' &&
            (base in this.constructor.defaults)) {
        var stub = {
            fn: repl,
            key: base,
            self: this,
            _op: 'set',
            deliver: function (spec, val, src) {
                if (this.key in val) {
                    this.fn.call(this.self, spec, val, src);
                }
            }
        };
        repl = stub;
        base = '';
    }
    // this will delay response if we have no state yet
    Syncable._pt._neutrals.on.call(this, spec, base, repl);
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.Model.prototype._neutrals.reoff"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype._neutrals.</span>reoff (spec, val, repl)](#apidoc.element.swarm.Model.prototype._neutrals.reoff)
- description and source-code
```javascript
reoff = function (spec, val, repl) {
    var idx = this.getListenerIndex(repl); //TODO ??? uplinks_only?
    if (idx > -1) {
        this._lstn.splice(idx, 1);
    }
    if (this._id) {
        this.checkUplink();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model.prototype._neutrals.reon"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype._neutrals.</span>reon (spec, filter, repl)](#apidoc.element.swarm.Model.prototype._neutrals.reon)
- description and source-code
```javascript
reon = function (spec, filter, repl) {
    if (filter) {  // a diff is requested
        var base = Spec.as(filter).tok('!');
        var diff = this.diff(base);
        if (diff) {
            repl.deliver(spec.set('.init'), diff, this);
        }
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Model.prototype._ops"></a>[module swarm.Model.prototype._ops](#apidoc.module.swarm.Model.prototype._ops)

#### <a name="apidoc.element.swarm.Model.prototype._ops.init"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype._ops.</span>init (spec, state, src)](#apidoc.element.swarm.Model.prototype._ops.init)
- description and source-code
```javascript
init = function (spec, state, src) {

    var tail = {}, // ops to be applied on top of the received state
        typeid = spec.filter('/#'),
        lstn = this._lstn,
        a_spec;
    this._lstn = []; // prevent events from being fired

    if (state._version/* && state._version !== '!0'*/) {
        // local changes may need to be merged into the received state
        if (this._oplog) {
            for (a_spec in this._oplog) {
                tail[a_spec] = this._oplog[a_spec];
            }
            this._oplog = {};
        }
        this._vector && (this._vector = undefined);
        // zero everything
        for (var key in this) {
            if (this.hasOwnProperty(key) && key.charAt(0) !== '_') {
                this[key] = undefined;
            }
        }
        // set default values
        this.reset();

        this.apply(state);
        this._version = state._version;

        state._oplog && (this._oplog = state._oplog); // FIXME copy
        state._vector && (this._vector = state._vector);
    }
    // add the received tail to the local one
    if (state._tail) {
        for (a_spec in state._tail) {
            tail[a_spec] = state._tail[a_spec];
        }
    }
    // appply the combined tail to the new state
    var specs = [];
    for (a_spec in tail) {
        specs.push(a_spec);
    }
    specs.sort().reverse();
    // there will be some replays, but those will be ignored
    while (a_spec = specs.pop()) {
        this.deliver(typeid.add(a_spec), tail[a_spec], this);
    }

    this._lstn = lstn;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Model.prototype._ops.set"></a>[function <span class="apidocSignatureSpan">swarm.Model.prototype._ops.</span>set (spec, value, repl)](#apidoc.element.swarm.Model.prototype._ops.set)
- description and source-code
```javascript
set = function (spec, value, repl) {
    var version = spec.version(),
        vermet = spec.filter('!.').toString();
    if (version < this._version.substr(1)) {
        this._oplog[vermet] = value;
        this.distillLog(); // may amend the value
        value = this._oplog[vermet];
    }
    value && this.apply(value);
}
```
- example usage
```shell
...

// 3.a. create an object
var someMouse = new Mouse();
// OR swarmHost.get('/Mouse');
// OR new Mouse({x:1, y:2});

// 4.a. a locally created object may be touched immediately
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
...
```



# <a name="apidoc.module.swarm.Pipe"></a>[module swarm.Pipe](#apidoc.module.swarm.Pipe)

#### <a name="apidoc.element.swarm.Pipe.Pipe"></a>[function <span class="apidocSignatureSpan">swarm.</span>Pipe (host, stream, opts)](#apidoc.element.swarm.Pipe.Pipe)
- description and source-code
```javascript
function Pipe(host, stream, opts) {
    var self = this;
    self.opts = opts || {};
    if (!stream || !host) {
        throw new Error('new Pipe(host,stream[,opts])');
    }
    self._id = null;
    self.host = host;
    // uplink/downlink state flag;
    //  true: this side initiated handshake >.on <.reon
    //  false: this side received handshake <.on >.reon
    //  undefined: nothing sent/received OR had a .reoff
    this.isOnSent = undefined;
    this.reconnectDelay = self.opts.reconnectDelay || 1000;
    self.serializer = self.opts.serializer || JSON;
    self.katimer = null;
    self.send_timer = null;
    self.lastSendTS = self.lastRecvTS = self.time();
    self.bundle = {};
    // don't send immediately, delay to bundle more messages
    self.delay = self.opts.delay || -1;
    //self.reconnectDelay = self.opts.reconnectDelay || 1000;
    if (typeof(stream.write) !== 'function') { // TODO nicer
        var url = stream.toString();
        var m = url.match(/(\w+):.*/);
        if (!m) {
            throw new Error('invalid url ' + url);
        }
        var proto = m[1].toLowerCase();
        var fn = env.streams[proto];
        if (!fn) {
            throw new Error('protocol not supported: ' + proto);
        }
        self.url = url;
        stream = new fn(url);
    }
    self.connect(stream);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Pipe.prototype"></a>[module swarm.Pipe.prototype](#apidoc.module.swarm.Pipe.prototype)

#### <a name="apidoc.element.swarm.Pipe.prototype.close"></a>[function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>close (error)](#apidoc.element.swarm.Pipe.prototype.close)
- description and source-code
```javascript
function pc(error) {
    env.log(dotClose, error ? 'error: ' + error : 'correct', this, this.host);
    if (error && this.host && this.url) {
        var uplink_uri = this.url,
            host = this.host,
            pipe_opts = this.opts;
        //reconnect delay for next disconnection
        pipe_opts.reconnectDelay = Math.min(30000, this.reconnectDelay << 1);
        // schedule a retry
        setTimeout(function () {
            host.connect(uplink_uri, pipe_opts);
        }, this.reconnectDelay);

        this.url = null; //to prevent second reconnection timer
    }
    if (this.host) {
        if (this.isOnSent !== undefined && this._id) {
            // emulate normal off
            var offspec = this.host.newEventSpec(this.isOnSent ? 'off' : 'reoff');
            this.host.deliver(offspec, '', this);
        }
        this.host = null; // can't pass any more messages
    }
    if (this.katimer) {
        clearInterval(this.katimer);
        this.katimer = null;
    }
    if (this.stream) {
        try {
            this.stream.close();
        } catch (ex) {}
        this.stream = null;
    }
    this._id = null;
}
```
- example usage
```shell
...
        }
    }, 1);
};

AsyncLoopbackConnection.prototype.close = function () {
    delete AsyncLoopbackConnection.pipes[this.id];
    var pair = this.pair();
    pair && pair.close();
    this.lstn.close && this.lstn.close();
};
...
```

#### <a name="apidoc.element.swarm.Pipe.prototype.connect"></a>[function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>connect (stream)](#apidoc.element.swarm.Pipe.prototype.connect)
- description and source-code
```javascript
function pc(stream) {
    var self = this;
    self.stream = stream;

    self.stream.on('data', function onMsg(data) {
        data = data.toString();
        env.trace && env.log(dotIn, data, this, this.host);
        self.lastRecvTS = self.time();
        var json = self.serializer.parse(data);
        try {
            self._id ? self.parseBundle(json) : self.parseHandshake(json);
        } catch (ex) {
            console.error('error processing message', ex, ex.stack);
            //this.deliver(this.host.newEventSpec('error'), ex.message);
            this.close();
        }
        self.reconnectDelay = self.opts.reconnectDelay || 1000;
    });

    self.stream.on('close', function onConnectionClosed(reason) {
        self.stream = null; // needs no further attention
        self.close("stream closed");
    });

    self.stream.on('error', function (err) {
        self.close('stream error event: ' + err);
    });

    self.katimer = setInterval(self.keepAliveFn.bind(self), (Pipe.TIMEOUT / 4 + Math.random() * 100) | 0);

    // NOPE client only finally, initiate handshake
    // self.host.connect(self);

}
```
- example usage
```shell
...
### Using the model on the client (app.js)

'''js
// 1. create local Host
var swarmHost = new Swarm.Host('unique_client_id');

// 2. connect to your server
swarmHost.connect('ws://localhost:8000/');

// 3.a. create an object
var someMouse = new Mouse();
// OR swarmHost.get('/Mouse');
// OR new Mouse({x:1, y:2});

// 4.a. a locally created object may be touched immediately
...
```

#### <a name="apidoc.element.swarm.Pipe.prototype.deliver"></a>[function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>deliver (spec, val, src)](#apidoc.element.swarm.Pipe.prototype.deliver)
- description and source-code
```javascript
function pd(spec, val, src) {
    var self = this;
    val && val.constructor === Spec && (val = val.toString());
    if (spec.type() === 'Host') {
        switch (spec.op()) {
        case 'reoff':
            setTimeout(function itsOverReally() {
                self.isOnSent = undefined;
                self.close();
            }, 1);
            break;
        case 'off':
            setTimeout(function tickingBomb() {
                self.close();
            }, 5000);
            break;
        case 'on':
            this.isOnSent = true;
        case 'reon':
            this.isOnSent = false;
        }
    }
    this.bundle[spec] = val === undefined ? null : val; // TODO aggregation
    if (this.delay === -1) {
        this.sendBundle();
    } else if (!this.send_timer) {
        var now = this.time(),
            gap = now - this.lastSendTS,
            timeout = gap > this.delay ? this.delay : this.delay - gap;
        this.send_timer = setTimeout(this.sendBundle.bind(this), timeout); // hmmm...
    } // else {} // just wait
}
```
- example usage
```shell
...
if (this.callbacks===null) { return; }
var that = this.owner || src;
for(var i=0; i<this.callbacks.length; i++) {
    var cb = this.callbacks[i];
    if (cb.constructor===Function) {
        cb.call(that,spec,value,src);
    } else {
        cb.deliver(spec,value,src);
    }
}
};

ProxyListener.prototype.on = function (callback) {
if (this.callbacks===null) { this.callbacks = []; }
this.callbacks.push(callback);
...
```

#### <a name="apidoc.element.swarm.Pipe.prototype.keepAliveFn"></a>[function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>keepAliveFn ()](#apidoc.element.swarm.Pipe.prototype.keepAliveFn)
- description and source-code
```javascript
keepAliveFn = function () {
    var now = this.time(),
        sinceRecv = now - this.lastRecvTS,
        sinceSend = now - this.lastSendTS;
    if (sinceSend > Pipe.TIMEOUT / 2) {
        this.sendBundle();
    }
    if (sinceRecv > Pipe.TIMEOUT) {
        this.close("stream timeout");
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Pipe.prototype.parseBundle"></a>[function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>parseBundle (bundle)](#apidoc.element.swarm.Pipe.prototype.parseBundle)
- description and source-code
```javascript
function pb(bundle) {
    var spec_list = [], spec, self = this;
    //parse specifiers
    for (spec in bundle) { spec && spec_list.push(new Spec(spec)); }
    spec_list.sort().reverse();
    while (spec = spec_list.pop()) {
        spec = Spec.as(spec);
        this.host.deliver(spec, bundle[spec], this);
        if (spec.type() === 'Host' && spec.op() === 'reoff') { //TODO check #id
            setTimeout(function () {
                self.isOnSent = undefined;
                self.close();
            }, 1);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Pipe.prototype.parseHandshake"></a>[function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>parseHandshake (handshake)](#apidoc.element.swarm.Pipe.prototype.parseHandshake)
- description and source-code
```javascript
function ph(handshake) {
    var spec, value, key;
    for (key in handshake) {
        spec = new Spec(key);
        value = handshake[key];
        break; // 8)-
    }
    if (!spec) {
        throw new Error('handshake has no spec');
    }
    if (spec.type() !== 'Host') {
        env.warn("non-Host handshake");
    }
    if (spec.id() === this.host._id) {
        throw new Error('self hs');
    }
    this._id = spec.id();
    var op = spec.op();
    var evspec = spec.set(this.host._id, '#');

    if (op in {on: 1, reon: 1, off: 1, reoff: 1}) {// access denied TODO
        this.host.deliver(evspec, value, this);
    } else {
        throw new Error('invalid handshake');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Pipe.prototype.sendBundle"></a>[function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>sendBundle ()](#apidoc.element.swarm.Pipe.prototype.sendBundle)
- description and source-code
```javascript
function pS() {
    var payload = this.serializer.stringify(this.bundle);
    this.bundle = {};
    if (!this.stream) {
        this.send_timer = null;
        return; // too late
    }

    try {
        env.trace && env.log(dotOut, payload, this, this.host);
        this.stream.write(payload);
        this.lastSendTS = this.time();
    } catch (ex) {
        env.error('stream error on write: ' + ex, ex.stack);
        if (this._id) {
            this.close('stream error', ex);
        }
    } finally {
        this.send_timer = null;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Pipe.prototype.spec"></a>[function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>spec ()](#apidoc.element.swarm.Pipe.prototype.spec)
- description and source-code
```javascript
spec = function () {
    return this._id ? new Spec('/Host#' + this._id) : '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Pipe.prototype.time"></a>[function <span class="apidocSignatureSpan">swarm.Pipe.prototype.</span>time ()](#apidoc.element.swarm.Pipe.prototype.time)
- description and source-code
```javascript
time = function () { return new Date().getTime(); }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.ProxyListener"></a>[module swarm.ProxyListener](#apidoc.module.swarm.ProxyListener)

#### <a name="apidoc.element.swarm.ProxyListener.ProxyListener"></a>[function <span class="apidocSignatureSpan">swarm.</span>ProxyListener ()](#apidoc.element.swarm.ProxyListener.ProxyListener)
- description and source-code
```javascript
function ProxyListener() {
    this.callbacks = null;
    this.owner = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.ProxyListener.prototype"></a>[module swarm.ProxyListener.prototype](#apidoc.module.swarm.ProxyListener.prototype)

#### <a name="apidoc.element.swarm.ProxyListener.prototype.deliver"></a>[function <span class="apidocSignatureSpan">swarm.ProxyListener.prototype.</span>deliver (spec, value, src)](#apidoc.element.swarm.ProxyListener.prototype.deliver)
- description and source-code
```javascript
deliver = function (spec, value, src) {
    if (this.callbacks===null) { return; }
    var that = this.owner || src;
    for(var i=0; i<this.callbacks.length; i++) {
        var cb = this.callbacks[i];
        if (cb.constructor===Function) {
            cb.call(that,spec,value,src);
        } else {
            cb.deliver(spec,value,src);
        }
    }
}
```
- example usage
```shell
...
if (this.callbacks===null) { return; }
var that = this.owner || src;
for(var i=0; i<this.callbacks.length; i++) {
    var cb = this.callbacks[i];
    if (cb.constructor===Function) {
        cb.call(that,spec,value,src);
    } else {
        cb.deliver(spec,value,src);
    }
}
};

ProxyListener.prototype.on = function (callback) {
if (this.callbacks===null) { this.callbacks = []; }
this.callbacks.push(callback);
...
```

#### <a name="apidoc.element.swarm.ProxyListener.prototype.off"></a>[function <span class="apidocSignatureSpan">swarm.ProxyListener.prototype.</span>off (callback)](#apidoc.element.swarm.ProxyListener.prototype.off)
- description and source-code
```javascript
off = function (callback) {
    if (this.callbacks===null) { return; }
    var i = this.callbacks.indexOf(callback);
    if (i!==-1) {
        this.callbacks.splice(i,1);
    } else {
        console.warn('listener unknown', callback);
    }
}
```
- example usage
```shell
...

/**
 * Unsubscribe from collections entries' events
 * @param {function(*)} callback
 * @this Set|Vector
 */
offObjectEvent: function (callback) {
    this._proxy.off(callback);
},

/**
 * Waits for collection to receive state from cache or uplink and then invokes passed callback
 *
 * @param {function()} callback
 * @this Set|Vector
...
```

#### <a name="apidoc.element.swarm.ProxyListener.prototype.on"></a>[function <span class="apidocSignatureSpan">swarm.ProxyListener.prototype.</span>on (callback)](#apidoc.element.swarm.ProxyListener.prototype.on)
- description and source-code
```javascript
on = function (callback) {
    if (this.callbacks===null) { this.callbacks = []; }
    this.callbacks.push(callback);
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```



# <a name="apidoc.module.swarm.ReactMixin"></a>[module swarm.ReactMixin](#apidoc.module.swarm.ReactMixin)

#### <a name="apidoc.element.swarm.ReactMixin.componentWillMount"></a>[function <span class="apidocSignatureSpan">swarm.ReactMixin.</span>componentWillMount ()](#apidoc.element.swarm.ReactMixin.componentWillMount)
- description and source-code
```javascript
componentWillMount = function () {
    var spec = this.props.spec || this.props.key;
    if (!Spec.is(spec)) {
        if (spec && this.constructor.modelType) {
            var id = spec;
            spec = new Spec(this.constructor.modelType,'/'); // TODO fn!!!
            spec = spec.add(id,'#');
        } else {
            throw new Error('not a specifier: '+spec+' at '+this._rootNodeID);
        }
    }
    this.sync = env.localhost.get(spec);
    this.setState({version:''});
    if (!env.isServer) {
        var sync = this.sync;
        sync.on('init', this); // TODO single listener
        sync.on(this);
        if (this.props.listenEntries) {
            sync.onObjectEvent(this);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.ReactMixin.componentWillUnmount"></a>[function <span class="apidocSignatureSpan">swarm.ReactMixin.</span>componentWillUnmount ()](#apidoc.element.swarm.ReactMixin.componentWillUnmount)
- description and source-code
```javascript
componentWillUnmount = function () {
    if (!env.isServer) {
        var sync = this.sync;
        sync.off(this);
        sync.off(this); // FIXME: remove after TODO: prevent second subscription
        if (this.props.listenEntries) {
            sync.offObjectEvent(this);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.ReactMixin.deliver"></a>[function <span class="apidocSignatureSpan">swarm.ReactMixin.</span>deliver (spec, val, source)](#apidoc.element.swarm.ReactMixin.deliver)
- description and source-code
```javascript
deliver = function (spec, val, source) {
    var sync = this.sync;
    var version = sync._version;
    if (this.props.listenEntries) {
        var opId = '!' + spec.version();
        if (version !== opId) {
            version = opId;
        }
    }
    this.setState({version: version});
}
```
- example usage
```shell
...
if (this.callbacks===null) { return; }
var that = this.owner || src;
for(var i=0; i<this.callbacks.length; i++) {
    var cb = this.callbacks[i];
    if (cb.constructor===Function) {
        cb.call(that,spec,value,src);
    } else {
        cb.deliver(spec,value,src);
    }
}
};

ProxyListener.prototype.on = function (callback) {
if (this.callbacks===null) { this.callbacks = []; }
this.callbacks.push(callback);
...
```

#### <a name="apidoc.element.swarm.ReactMixin.shouldComponentUpdate"></a>[function <span class="apidocSignatureSpan">swarm.ReactMixin.</span>shouldComponentUpdate (nextProps, nextState)](#apidoc.element.swarm.ReactMixin.shouldComponentUpdate)
- description and source-code
```javascript
shouldComponentUpdate = function (nextProps, nextState) {
    return this.props !== nextProps || this.state.version !== nextState.version;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.SecondPreciseClock"></a>[module swarm.SecondPreciseClock](#apidoc.module.swarm.SecondPreciseClock)

#### <a name="apidoc.element.swarm.SecondPreciseClock.SecondPreciseClock"></a>[function <span class="apidocSignatureSpan">swarm.</span>SecondPreciseClock (processId, timeOffsetMs)](#apidoc.element.swarm.SecondPreciseClock.SecondPreciseClock)
- description and source-code
```javascript
SecondPreciseClock = function (processId, timeOffsetMs) {
    if (!Spec.reTok.test(processId)) {
        throw new Error('invalid process id: '+processId);
    }
    this.id = processId;
    // sometimes we assume our local clock has some offset
    this.clockOffsetMs = 0;
    this.lastTimestamp = '';
    // although we try hard to use wall clock time, we must
    // obey Lamport logical clock rules, in particular our
    // timestamps must be greater than any other timestamps
    // previously seen
    this.lastTimeSeen = 0;
    this.lastSeqSeen = 0;
    if (timeOffsetMs) {
        this.clockOffsetMs = timeOffsetMs;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.SecondPreciseClock.prototype"></a>[module swarm.SecondPreciseClock.prototype](#apidoc.module.swarm.SecondPreciseClock.prototype)

#### <a name="apidoc.element.swarm.SecondPreciseClock.prototype.adjustTime"></a>[function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>adjustTime (trueMs)](#apidoc.element.swarm.SecondPreciseClock.prototype.adjustTime)
- description and source-code
```javascript
adjustTime = function (trueMs) {
    var localTime = this.ms();
    var clockOffsetMs = trueMs - localTime;
    this.clockOffsetMs = clockOffsetMs;
    var lastTS = this.lastTimeSeen;
    this.lastTimeSeen = 0;
    this.lastSeqSeen = 0;
    this.lastTimestamp = '';
    if ( this.seconds()+1 < lastTS ) {
        console.error("risky clock reset",this.lastTimestamp);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.SecondPreciseClock.prototype.checkTimestamp"></a>[function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>checkTimestamp (ts)](#apidoc.element.swarm.SecondPreciseClock.prototype.checkTimestamp)
- description and source-code
```javascript
function see(ts) {
    if (ts<this.lastTimestamp) { return true; }
    var parsed = this.parseTimestamp(ts);
    if (parsed.time<this.lastTimeSeen) { return true; }
    var sec = this.seconds();
    if (parsed.time>sec+1) {
        return false; // back to the future
    }
    this.lastTimeSeen = parsed.time;
    this.lastSeqSeen = parsed.seq;
    return true;
}
```
- example usage
```shell
...
                        seqi = 1; // FIXME repeat ids, double insert
                    }
                }
            }
        }
    }
    if (genTs) {
        this._host.clock.checkTimestamp(genTs);
    }
    this.weave = w1.join('');
    this.ids = w4;
    this.rebuild();
},
remove: function (spec, rm, src) {
    var w1 = [], w4 = [];
...
```

#### <a name="apidoc.element.swarm.SecondPreciseClock.prototype.issueTimestamp"></a>[function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>issueTimestamp ()](#apidoc.element.swarm.SecondPreciseClock.prototype.issueTimestamp)
- description and source-code
```javascript
function time() {
    var res = this.seconds();
    if (this.lastTimeSeen>res) { res = this.lastTimeSeen; }
    if (res>this.lastTimeSeen) { this.lastSeqSeen = -1; }
    this.lastTimeSeen = res;
    var seq = ++this.lastSeqSeen;
    if (seq>=(1<<12)) {throw new Error('max event freq is 4000Hz');}

    var baseTimeSeq = Spec.int2base(res, 5);
    if (seq>0) { baseTimeSeq+=Spec.int2base(seq, 2); }

    this.lastTimestamp = baseTimeSeq + '+' + this.id;
    return this.lastTimestamp;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.SecondPreciseClock.prototype.ms"></a>[function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>ms ()](#apidoc.element.swarm.SecondPreciseClock.prototype.ms)
- description and source-code
```javascript
ms = function () {
    var millis = new Date().getTime();
    millis -= SecondPreciseClock.EPOCH;
    return millis;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.SecondPreciseClock.prototype.parseTimestamp"></a>[function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>parseTimestamp (ts)](#apidoc.element.swarm.SecondPreciseClock.prototype.parseTimestamp)
- description and source-code
```javascript
function parse(ts) {
    var m = ts.match(Spec.reTokExt);
    if (!m) {throw new Error('malformed timestamp: '+ts);}
    var timeseq=m[1]; //, process=m[2];
    var time = timeseq.substr(0,5), seq = timeseq.substr(5);
    if (seq&&seq.length!==2) {
        throw new Error('malformed timestamp value: '+timeseq);
    }
    return {
        time: Spec.base2int(time),
        seq: seq ? Spec.base2int(seq) : 0
    };
}
```
- example usage
```shell
...
        seq: Spec.base2int(m[1]),
        process: m[2]
    };
};

/** Lamport partial order  imperfect semi-logical*/
LamportClock.prototype.checkTimestamp = function see (ts) {
    var parsed = this.parseTimestamp(ts);
    if (parsed.seq >= this.seq) {
        this.seq = parsed.seq + 1;
    }
    return true;
};

LamportClock.prototype.time2date = function () {
...
```

#### <a name="apidoc.element.swarm.SecondPreciseClock.prototype.seconds"></a>[function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>seconds ()](#apidoc.element.swarm.SecondPreciseClock.prototype.seconds)
- description and source-code
```javascript
seconds = function () {
    var millis = this.ms();
    millis += this.clockOffsetMs;
    return (millis/1000) | 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.SecondPreciseClock.prototype.timestamp2date"></a>[function <span class="apidocSignatureSpan">swarm.SecondPreciseClock.prototype.</span>timestamp2date (ts)](#apidoc.element.swarm.SecondPreciseClock.prototype.timestamp2date)
- description and source-code
```javascript
timestamp2date = function (ts) {
    var parsed = this.parseTimestamp(ts);
    var millis = parsed.time * 1000 + SecondPreciseClock.EPOCH;
    return new Date(millis);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Set"></a>[module swarm.Set](#apidoc.module.swarm.Set)

#### <a name="apidoc.element.swarm.Set.Set"></a>[function <span class="apidocSignatureSpan">swarm.</span>Set ()](#apidoc.element.swarm.Set.Set)
- description and source-code
```javascript
function SomeSyncable() {
    return parent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set._super"></a>[function <span class="apidocSignatureSpan">swarm.Set.</span>_super ()](#apidoc.element.swarm.Set._super)
- description and source-code
```javascript
function Syncable() {
    // listeners represented as objects that have deliver() method
    this._lstn = [',']; // we unshift() uplink listeners and push() downlinks
    // ...so _lstn is like [server1, server2, storage, ',', view, listener]
    // The most correct way to specify a version is the version vector,
    // but that one may consume more space than the data itself in some cases.
    // Hence, _version is not a fully specified version vector (see version()
    // instead). _version is essentially is the greatest operation timestamp
    // (Lamport-like, i.e. "time+source"), sometimes amended with additional
    // timestamps. Its main features:
    // (1) changes once the object's state changes
    // (2) does it monotonically (in the alphanum order sense)
    this._version = '';
    // make sense of arguments
    var args = Array.prototype.slice.call(arguments);
    this._host = (args.length && args[args.length - 1]._type === 'Host') ?
            args.pop() : env.localhost;
    if (Spec.is(args[0])) {
        this._id = new Spec(args.shift()).id() || this._host.time();
    } else if (typeof(args[0]) === 'string') {
        this._id = args.shift(); // TODO format
    } else {
        this._id = this._host.time();
        this._version = '!0'; // may apply state in the constructor, see Model
    }
    //var state = args.length ? args.pop() : (fresh?{}:undefined);
    // register with the host
    var doubl = this._host.register(this);
    if (doubl !== this) { return doubl; }
    // locally created objects get state immediately
    // (while external-id objects need to query uplinks)
<span class="apidocCodeCommentSpan">    /*if (fresh && state) {
     state._version = '!'+this._id;
     var pspec = this.spec().add(state._version).add('.init');
     this.deliver(pspec,state,this._host);
     }*/
</span>    this.reset();
    // find uplinks, subscribe
    this.checkUplink();
    // TODO inplement state push
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.addReaction"></a>[function <span class="apidocSignatureSpan">swarm.Set.</span>addReaction (op, fn)](#apidoc.element.swarm.Set.addReaction)
- description and source-code
```javascript
addReaction = function (op, fn) {
    var reactions = this.prototype._reactions;
    var list = reactions[op];
    list || (list = reactions[op] = []);
    list.push(fn);
    return {op: op, fn: fn};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.extend"></a>[function <span class="apidocSignatureSpan">swarm.Set.</span>extend (fn, own)](#apidoc.element.swarm.Set.extend)
- description and source-code
```javascript
extend = function (fn, own) {
    var parent = this, fnid;
    if (fn.constructor !== Function) {
        var id = fn.toString();
        fn = function SomeSyncable() {
            return parent.apply(this, arguments);
        };
        fnid = id; // if only it worked
    } else { // please call Syncable.constructor.apply(this,args) in your constructor
        fnid = fnname(fn);
    }

    // inheritance trick from backbone.js
    var SyncProto = function () {
        this.constructor = fn;
        this._neutrals = {};
        this._ops = {};
        this._reactions = {};

        var event,
            name;
        if (parent._pt) {
            //copy _neutrals & _ops from parent
            for (event in parent._pt._neutrals) {
                this._neutrals[event] = parent._pt._neutrals[event];
            }
            for (event in parent._pt._ops) {
                this._ops[event] = parent._pt._ops[event];
            }
        }

        // "Methods" are serialized, logged and delivered to replicas
        for (name in own.ops || {}) {
            if (Syncable.reMethodName.test(name)) {
                this._ops[name] = own.ops[name];
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid op name:',name);
            }
        }

        // "Neutrals" don't change the state
        for (name in own.neutrals || {}) {
            if (Syncable.reMethodName.test(name)) {
                this._neutrals[name] = own.neutrals[name];
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid neutral op name:',name);
            }
        }

        // "Remotes" are serialized and sent upstream (like RPC calls)
        for (name in own.remotes || {}) {
            if (Syncable.reMethodName.test(name)) {
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid rpc name:',name);
            }
        }

        // add mixins
        (own.mixins || []).forEach(function (mixin) {
            for (var name in mixin) {
                this[name] = mixin[name];
            }
        }, this);

        // add other members
        for (name in own) {
            if (Syncable.reMethodName.test(name)) {
                var memberType = own[name].constructor;
                if (memberType === Function) { // non-op method
                    // these must change state ONLY by invoking ops
                    this[name] = own[name];
                } else if (memberType===String || memberType===Number) {
                    this[name] = own[name]; // some static constant, OK
                } else if (name in Syncable.memberClasses) {
                    // see above
                    continue;
                } else {
                    console.warn('invalid member:',name,memberType);
                }
            } else {
                console.warn('invalid member name:',name);
            }
        }

        // add reactions
        for (name in own.reactions || {}) {
            var reaction = own.reactions[name];
            if (!reaction) { continue; }

            switch (typeof reaction) {
            case 'function':
                // handler-function
                this._reactions[name] = [reaction];
                break;
            case 'string':
                // handler-method name
                this._reactions[name] = [this[name]];
                break;
            default:
                if (reaction.constructor === Array) {
                    // array of handlers
                    this._reactions[name] = reaction.map(function (item) {
                        switch (typeof item) {
                        case 'function':
                            return item;
                        case 'string':
                            return this[item];
                        default:
                            throw new Error('unexpected reaction type');
                        }
                    }, this);
                } else {
                    throw new Error('unex ...
```
- example usage
```shell
...
these demos are normally online at http://ppyr.us and http://ppyr.us:8001/demo3/index.html respectively.

### Creating your first simple synchronized type

'''js
var Swarm = require('swarm');

var Mouse = Swarm.Model.extend('Mouse', {
    defaults: {
        name: 'Mickey',
        x: 0,
        y: 0
    }
});
...
```

#### <a name="apidoc.element.swarm.Set.removeReaction"></a>[function <span class="apidocSignatureSpan">swarm.Set.</span>removeReaction (handle)](#apidoc.element.swarm.Set.removeReaction)
- description and source-code
```javascript
removeReaction = function (handle) {
    var op = handle.op,
        fn = handle.fn,
        list = this.prototype._reactions[op],
        i = list.indexOf(fn);
    if (i === -1) {
        throw new Error('reaction unknown');
    }
    list[i] = undefined; // such a peculiar pattern not to mess up out-of-callback removal
    while (list.length && !list[list.length - 1]) {
        list.pop();
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Set.prototype"></a>[module swarm.Set.prototype](#apidoc.module.swarm.Set.prototype)

#### <a name="apidoc.element.swarm.Set.prototype.addObject"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>addObject (obj)](#apidoc.element.swarm.Set.prototype.addObject)
- description and source-code
```javascript
addObject = function (obj) {
    var specs = {};
    specs[obj.spec()] = 1;
    this.change(specs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.callReactions"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>callReactions (spec, value, src)](#apidoc.element.swarm.Set.prototype.callReactions)
- description and source-code
```javascript
callReactions = function (spec, value, src) {
    var superReactions = syncProto._super.callReactions;
    if ('function' === typeof superReactions) {
        superReactions.call(this, spec, value, src);
    }
    var r = syncProto._reactions[spec.op()];
    if (r) {
        r.constructor !== Array && (r = [r]);
        for (var i = 0; i < r.length; i++) {
            r[i] && r[i].call(this, spec, value, src);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.change"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>change ()](#apidoc.element.swarm.Set.prototype.change)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.constructor"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>constructor ()](#apidoc.element.swarm.Set.prototype.constructor)
- description and source-code
```javascript
function SomeSyncable() {
    return parent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.distillLog"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>distillLog ()](#apidoc.element.swarm.Set.prototype.distillLog)
- description and source-code
```javascript
distillLog = function () {
    // explain
    var sets = [],
        cumul = {},
        heads = {},
        spec;
    for (var s in this._oplog) {
        spec = new Spec(s);
        //if (spec.op() === 'set') {
        sets.push(spec);
        //}
    }
    sets.sort();
    for (var i = sets.length - 1; i >= 0; i--) {
        spec = sets[i];
        var val = this._oplog[spec],
            notempty = false;
        for (var field in val) {
            if (field in cumul) {
                delete val[field];
            } else {
                notempty = cumul[field] = val[field]; //store last value of the field
            }
        }
        var source = spec.source();
        notempty || (heads[source] && delete this._oplog[spec]);
        heads[source] = true;
    }
    return cumul;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.distillOp"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>distillOp (spec, val)](#apidoc.element.swarm.Set.prototype.distillOp)
- description and source-code
```javascript
distillOp = function (spec, val) {
    if (spec.version() > this._version) {
        return val; // no concurrent op
    }
    var opkey = spec.filter('!.');
    this._oplog[opkey] = val;
    this.distillLog(); // may amend the value
    return this._oplog[opkey] || {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.every"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>every (cb, thisArg)](#apidoc.element.swarm.Set.prototype.every)
- description and source-code
```javascript
every = function (cb, thisArg) {
    var index = 0;
    for (var spec in this._objects) {
        if (!cb.call(thisArg, this._objects[spec], index++)) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.filter"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>filter (cb, thisArg)](#apidoc.element.swarm.Set.prototype.filter)
- description and source-code
```javascript
filter = function (cb, thisArg) {
    var res = [];
    this.forEach(function (entry, idx) {
        if (cb.call(thisArg, entry, idx)) {
            res.push(entry);
        }
    });
    return res;
}
```
- example usage
```shell
...
 *
 * @param {function()} callback
 * @this Set|Vector
 */
onObjectStateReady: function (callback) { // TODO timeout ?
    var self = this;
    function checker() {
        var notInitedYet = self.filter(function (entry) {
            return !entry._version;
        });
        if (!notInitedYet.length) {
            // all entries are inited
            callback();
        } else {
            // wait for some entry not ready yet
...
```

#### <a name="apidoc.element.swarm.Set.prototype.forEach"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>forEach (cb, thisArg)](#apidoc.element.swarm.Set.prototype.forEach)
- description and source-code
```javascript
forEach = function (cb, thisArg) {
    var index = 0;
    for (var spec in this._objects) {
        cb.call(thisArg, this._objects[spec], index++);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.get"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>get (key_spec)](#apidoc.element.swarm.Set.prototype.get)
- description and source-code
```javascript
get = function (key_spec) {
    key_spec = new Spec(key_spec).filter('/#');
    if (key_spec.pattern() !== '/#') {
        throw new Error("invalid spec");
    }
    return this._objects[key_spec];
}
```
- example usage
```shell
...
var swarmHost = new Swarm.Host('unique_client_id');

// 2. connect to your server
swarmHost.connect('ws://localhost:8000/');

// 3.a. create an object
var someMouse = new Mouse();
// OR swarmHost.get('/Mouse');
// OR new Mouse({x:1, y:2});

// 4.a. a locally created object may be touched immediately
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
...
```

#### <a name="apidoc.element.swarm.Set.prototype.list"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>list (order)](#apidoc.element.swarm.Set.prototype.list)
- description and source-code
```javascript
list = function (order) {
    var ret = [];
    for (var key in this._objects) {
        ret.push(this._objects[key]);
    }
    ret.sort(order);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.map"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>map (cb, thisArg)](#apidoc.element.swarm.Set.prototype.map)
- description and source-code
```javascript
map = function (cb, thisArg) {
    var res = [];
    this.forEach(function (entry, idx) {
        res.push(cb.call(thisArg, entry, idx));
    });
    return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.offObjectEvent"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>offObjectEvent (callback)](#apidoc.element.swarm.Set.prototype.offObjectEvent)
- description and source-code
```javascript
offObjectEvent = function (callback) {
    this._proxy.off(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.onObjectEvent"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>onObjectEvent (callback)](#apidoc.element.swarm.Set.prototype.onObjectEvent)
- description and source-code
```javascript
onObjectEvent = function (callback) {
    this._proxy.owner = this;
    this._proxy.on(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.onObjectStateReady"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>onObjectStateReady (callback)](#apidoc.element.swarm.Set.prototype.onObjectStateReady)
- description and source-code
```javascript
onObjectStateReady = function (callback) { // TODO timeout ?
    var self = this;
    function checker() {
        var notInitedYet = self.filter(function (entry) {
            return !entry._version;
        });
        if (!notInitedYet.length) {
            // all entries are inited
            callback();
        } else {
            // wait for some entry not ready yet
            var randomIdx = (Math.random() * (notInitedYet.length - 1)) | 0;
            notInitedYet[randomIdx].once('init', checker);
        }
    }
    if (this._version) {
        checker();
    } else {
        this.once('init', checker);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.pojo"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>pojo ()](#apidoc.element.swarm.Set.prototype.pojo)
- description and source-code
```javascript
pojo = function () {
    // invoke super.pojo()
    var result = Syncable._pt.pojo.apply(this, arguments);
    result.entries = Object.keys(this._objects);
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.removeObject"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>removeObject (obj)](#apidoc.element.swarm.Set.prototype.removeObject)
- description and source-code
```javascript
removeObject = function (obj) {
    var spec = obj._id ? obj.spec() : new Spec(obj).filter('/#');
    if (spec.pattern() !== '/#') {
        throw new Error('invalid spec: ' + spec);
    }
    var specs = {};
    specs[spec] = 0;
    this.change(specs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype.validate"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype.</span>validate (spec, val, src)](#apidoc.element.swarm.Set.prototype.validate)
- description and source-code
```javascript
validate = function (spec, val, src) {
    if (spec.op() !== 'change') {
        return '';
    }

    for (var key_spec in val) {
        // member spec validity
        if (Spec.pattern(key_spec) !== '/#') {
            return 'invalid spec: ' + key_spec;
        }
    }
    return '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Set.prototype._neutrals"></a>[module swarm.Set.prototype._neutrals](#apidoc.module.swarm.Set.prototype._neutrals)

#### <a name="apidoc.element.swarm.Set.prototype._neutrals.error"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype._neutrals.</span>error (spec, val, repl)](#apidoc.element.swarm.Set.prototype._neutrals.error)
- description and source-code
```javascript
error = function (spec, val, repl) {
    console.error('something failed:', spec, val, '@', (repl && repl._id));
}
```
- example usage
```shell
...
        this.buf = buf; //will wait for "open"
    }
    ws.on('close', function () { ln.close && ln.close(); });
    ws.on('data', function (msg) {
        try {
            ln.data && ln.data(msg);
        } catch (ex) {
            console.error('message processing fails', ex);
            ln.error && ln.error(ex.message);
        }
    });
}

module.exports = SockJSStream;
...
```

#### <a name="apidoc.element.swarm.Set.prototype._neutrals.off"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype._neutrals.</span>off (spec, val, repl)](#apidoc.element.swarm.Set.prototype._neutrals.off)
- description and source-code
```javascript
off = function (spec, val, repl) {
    var idx = this.getListenerIndex(repl); //TODO ??? uplinks_only?
    if (idx > -1) {
        this._lstn.splice(idx, 1);
    }
}
```
- example usage
```shell
...

/**
 * Unsubscribe from collections entries' events
 * @param {function(*)} callback
 * @this Set|Vector
 */
offObjectEvent: function (callback) {
    this._proxy.off(callback);
},

/**
 * Waits for collection to receive state from cache or uplink and then invokes passed callback
 *
 * @param {function()} callback
 * @this Set|Vector
...
```

#### <a name="apidoc.element.swarm.Set.prototype._neutrals.on"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype._neutrals.</span>on (spec, filter, repl)](#apidoc.element.swarm.Set.prototype._neutrals.on)
- description and source-code
```javascript
on = function (spec, filter, repl) {   // WELL  on() is not an op, right?
    // if no listener is supplied then the object is only
    // guaranteed to exist till the next Host.gc() run
    if (!repl) { return; }

    var self = this;
    // stateless objects fire no events; essentially, on() is deferred
    if (!this._version && filter) { // TODO solidify
        this._lstn.push({
            _op: 'reon',
            _src: repl,
            deliver: function () {
                var i = self._lstn.indexOf(this);
                self._lstn.splice(i, 1);
                self.deliver(spec, filter, repl);
            }
        });
        return; // defer this call till uplinks are ready
    }
    // make all listeners uniform objects
    if (repl.constructor === Function) {
        repl = {
            sink: repl,
            that: this,
            deliver: function () { // .deliver is invoked on an event
                this.sink.apply(this.that, arguments);
            }
        };
    }

    if (filter) {
        filter = new Spec(filter, '.');
        var baseVersion = filter.filter('!'),
            filter_by_op = filter.get('.');

        if (filter_by_op === 'init') {
            var diff_if_needed = baseVersion ? this.diff(baseVersion) : '';
            repl.deliver(spec.set('.init'), diff_if_needed, this); //??
            // FIXME use once()
            return;
        }
        if (filter_by_op) {
            repl = {
                sink: repl,
                _op: filter_by_op,
                deliver: function deliverWithFilter(spec, val, src) {
                    if (spec.op() === filter_by_op) {
                        this.sink.deliver(spec, val, src);
                    }
                }
            };
        }

        if (!baseVersion.isEmpty()) {
            var diff = this.diff(baseVersion);
            diff && repl.deliver(spec.set('.init'), diff, this); // 2downlink
            repl.deliver(spec.set('.reon'), this.version().toString(), this);
        }
    }

    this._lstn.push(repl);
    // TODO repeated subscriptions: send a diff, otherwise ignore
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.Set.prototype._neutrals.reoff"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype._neutrals.</span>reoff (spec, val, repl)](#apidoc.element.swarm.Set.prototype._neutrals.reoff)
- description and source-code
```javascript
reoff = function (spec, val, repl) {
    var idx = this.getListenerIndex(repl); //TODO ??? uplinks_only?
    if (idx > -1) {
        this._lstn.splice(idx, 1);
    }
    if (this._id) {
        this.checkUplink();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype._neutrals.reon"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype._neutrals.</span>reon (spec, filter, repl)](#apidoc.element.swarm.Set.prototype._neutrals.reon)
- description and source-code
```javascript
reon = function (spec, filter, repl) {
    if (filter) {  // a diff is requested
        var base = Spec.as(filter).tok('!');
        var diff = this.diff(base);
        if (diff) {
            repl.deliver(spec.set('.init'), diff, this);
        }
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Set.prototype._ops"></a>[module swarm.Set.prototype._ops](#apidoc.module.swarm.Set.prototype._ops)

#### <a name="apidoc.element.swarm.Set.prototype._ops.change"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype._ops.</span>change (spec, value, repl)](#apidoc.element.swarm.Set.prototype._ops.change)
- description and source-code
```javascript
change = function (spec, value, repl) {
    value = this.distillOp(spec, value);
    var key_spec;
    for (key_spec in value) {
        if (value[key_spec] === 1) {
            if (!this._objects[key_spec]) { // only if object not in the set
                this._objects[key_spec] = this._host.get(key_spec);
                this._objects[key_spec].on(this._proxy);
            }
        } else if (value[key_spec] === 0) {
            if (this._objects[key_spec]) {
                this._objects[key_spec].off(this._proxy);
                delete this._objects[key_spec];
            }
        } else {
            env.log(this.spec(), 'unexpected val', JSON.stringify(value));
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Set.prototype._ops.init"></a>[function <span class="apidocSignatureSpan">swarm.Set.prototype._ops.</span>init (spec, state, src)](#apidoc.element.swarm.Set.prototype._ops.init)
- description and source-code
```javascript
init = function (spec, state, src) {

    var tail = {}, // ops to be applied on top of the received state
        typeid = spec.filter('/#'),
        lstn = this._lstn,
        a_spec;
    this._lstn = []; // prevent events from being fired

    if (state._version/* && state._version !== '!0'*/) {
        // local changes may need to be merged into the received state
        if (this._oplog) {
            for (a_spec in this._oplog) {
                tail[a_spec] = this._oplog[a_spec];
            }
            this._oplog = {};
        }
        this._vector && (this._vector = undefined);
        // zero everything
        for (var key in this) {
            if (this.hasOwnProperty(key) && key.charAt(0) !== '_') {
                this[key] = undefined;
            }
        }
        // set default values
        this.reset();

        this.apply(state);
        this._version = state._version;

        state._oplog && (this._oplog = state._oplog); // FIXME copy
        state._vector && (this._vector = state._vector);
    }
    // add the received tail to the local one
    if (state._tail) {
        for (a_spec in state._tail) {
            tail[a_spec] = state._tail[a_spec];
        }
    }
    // appply the combined tail to the new state
    var specs = [];
    for (a_spec in tail) {
        specs.push(a_spec);
    }
    specs.sort().reverse();
    // there will be some replays, but those will be ignored
    while (a_spec = specs.pop()) {
        this.deliver(typeid.add(a_spec), tail[a_spec], this);
    }

    this._lstn = lstn;

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.SharedWebStorage"></a>[module swarm.SharedWebStorage](#apidoc.module.swarm.SharedWebStorage)

#### <a name="apidoc.element.swarm.SharedWebStorage.SharedWebStorage"></a>[function <span class="apidocSignatureSpan">swarm.</span>SharedWebStorage (id, options)](#apidoc.element.swarm.SharedWebStorage.SharedWebStorage)
- description and source-code
```javascript
function SharedWebStorage(id, options) {
    this.options = options || {};
    this.lstn = {};
    this._id = id;
    this.tails = {};
    this.store = this.options.persistent ?
        window.localStorage : window.sessionStorage;

    this.loadLog();
    this.installListeners();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.SharedWebStorage.prototype"></a>[module swarm.SharedWebStorage.prototype](#apidoc.module.swarm.SharedWebStorage.prototype)

#### <a name="apidoc.element.swarm.SharedWebStorage.prototype.installListeners"></a>[function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>installListeners ()](#apidoc.element.swarm.SharedWebStorage.prototype.installListeners)
- description and source-code
```javascript
installListeners = function () {
    var self = this;
    function onStorageChange(ev) {
        if (Spec.is(ev.key) && ev.newValue) {
            self.onOp(new Spec(ev.key), JSON.parse(ev.newValue));
        }
    }
    window.addEventListener('storage', onStorageChange, false);
}
```
- example usage
```shell
...
    this.lstn = {};
    this._id = id;
    this.tails = {};
    this.store = this.options.persistent ?
        window.localStorage : window.sessionStorage;

    this.loadLog();
    this.installListeners();
}

SharedWebStorage.prototype = new Storage();
SharedWebStorage.prototype.isRoot = false;
module.exports = SharedWebStorage;
...
```

#### <a name="apidoc.element.swarm.SharedWebStorage.prototype.loadLog"></a>[function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>loadLog ()](#apidoc.element.swarm.SharedWebStorage.prototype.loadLog)
- description and source-code
```javascript
loadLog = function () {
    // scan/sort specs for existing records
    var store = this.store;
    var ti;
    for (var i = 0; i < store.length; i++) {
        var key = store.key(i);
        if (!Spec.is(key)) { continue; }
        var spec = new Spec(key);
        if (spec.pattern() !== '/#!.') {
            continue; // ops only
        }
        ti = spec.filter('/#');
        var tail = this.tails[ti];
        if (!tail) {
            tail = this.tails[ti] = [];
        }
        tail.push(spec.filter('!.'));
    }
    for (ti in this.tails) {
        this.tails[ti].sort();
    }
}
```
- example usage
```shell
...
    this.options = options || {};
    this.lstn = {};
    this._id = id;
    this.tails = {};
    this.store = this.options.persistent ?
        window.localStorage : window.sessionStorage;

    this.loadLog();
    this.installListeners();
}

SharedWebStorage.prototype = new Storage();
SharedWebStorage.prototype.isRoot = false;
module.exports = SharedWebStorage;
...
```

#### <a name="apidoc.element.swarm.SharedWebStorage.prototype.onOp"></a>[function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>onOp (spec, value)](#apidoc.element.swarm.SharedWebStorage.prototype.onOp)
- description and source-code
```javascript
onOp = function (spec, value) {
    var ti = spec.filter('/#');
    var vo = spec.filter('!.');
    if (!vo.toString()) {
        return; // state, not an op
    }
    var tail = this.tails[ti];
    if (!tail) {
        tail = this.tails[ti] = [];
    } else if (tail.indexOf(vo)!==-1) {
        return; // replay
    }
    tail.push(vo);
    this.emit(spec,value);
}
```
- example usage
```shell
...
};


SharedWebStorage.prototype.installListeners = function () {
    var self = this;
    function onStorageChange(ev) {
        if (Spec.is(ev.key) && ev.newValue) {
            self.onOp(new Spec(ev.key), JSON.parse(ev.newValue));
        }
    }
    window.addEventListener('storage', onStorageChange, false);
};


SharedWebStorage.prototype.loadLog = function () {
...
```

#### <a name="apidoc.element.swarm.SharedWebStorage.prototype.readOps"></a>[function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>readOps (ti, callback)](#apidoc.element.swarm.SharedWebStorage.prototype.readOps)
- description and source-code
```javascript
readOps = function (ti, callback) {
    var tail = this.tails[ti];
    var parsed = null;
    for(var k=0; tail && k<tail.length; k++) {
        var spec = tail[k];
        var value = this.store.getItem(ti+spec);
        if (!value) {continue;} // it happens
        parsed = parsed || {};
        parsed[spec] = JSON.parse(value);
    }
    callback(null, parsed);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.SharedWebStorage.prototype.readState"></a>[function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>readState (spec, callback)](#apidoc.element.swarm.SharedWebStorage.prototype.readState)
- description and source-code
```javascript
readState = function (spec, callback) {
    spec = new Spec(spec);
    var ti = spec.filter('/#');
    var state = this.store.getItem(ti);
    callback(null, (state&&JSON.parse(state)) || null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.SharedWebStorage.prototype.writeOp"></a>[function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>writeOp (spec, value, src)](#apidoc.element.swarm.SharedWebStorage.prototype.writeOp)
- description and source-code
```javascript
function wsOp(spec, value, src) {
    var ti = spec.filter('/#');
    var vm = spec.filter('!.');
    var tail = this.tails[ti] || (this.tails[ti] = []);
    tail.push(vm);
    var json = JSON.stringify(value);
    this.store.setItem(spec, json);
    if (this.options.trigger) {
        var otherStore = !this.options.persistent ?
            window.localStorage : window.sessionStorage;
        if (!otherStore.getItem(spec)) {
            otherStore.setItem(spec,json);
            otherStore.removeItem(spec,json);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.SharedWebStorage.prototype.writeState"></a>[function <span class="apidocSignatureSpan">swarm.SharedWebStorage.prototype.</span>writeState (spec, state, src)](#apidoc.element.swarm.SharedWebStorage.prototype.writeState)
- description and source-code
```javascript
function wsPatch(spec, state, src) {
    var ti = spec.filter('/#');
    this.store.setItem(ti, JSON.stringify(state));
    var tail = this.tails[ti];
    if (tail) {
        for(var k=0; k<tail.length; k++) {
            this.store.removeItem(ti + tail[k]);
        }
        delete this.tails[ti];
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.SockJSServerStream"></a>[module swarm.SockJSServerStream](#apidoc.module.swarm.SockJSServerStream)

#### <a name="apidoc.element.swarm.SockJSServerStream.SockJSServerStream"></a>[function <span class="apidocSignatureSpan">swarm.</span>SockJSServerStream (ws)](#apidoc.element.swarm.SockJSServerStream.SockJSServerStream)
- description and source-code
```javascript
function SockJSStream(ws) {
    var ln = this.lstn = {},
        buf = [];

    if (typeof ws === 'string') { // url passed
        throw new Error('client-side connections not supported yet');
    }
    this.ws = ws;
    if (ws.readyState !== 1/*WebSocket.OPEN*/) {
        this.buf = buf; //will wait for "open"
    }
    ws.on('close', function () { ln.close && ln.close(); });
    ws.on('data', function (msg) {
        try {
            ln.data && ln.data(msg);
        } catch (ex) {
            console.error('message processing fails', ex);
            ln.error && ln.error(ex.message);
        }
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.SockJSServerStream.prototype"></a>[module swarm.SockJSServerStream.prototype](#apidoc.module.swarm.SockJSServerStream.prototype)

#### <a name="apidoc.element.swarm.SockJSServerStream.prototype.on"></a>[function <span class="apidocSignatureSpan">swarm.SockJSServerStream.prototype.</span>on (evname, fn)](#apidoc.element.swarm.SockJSServerStream.prototype.on)
- description and source-code
```javascript
on = function (evname, fn) {
    if (evname in this.lstn) {
        throw new Error('not supported');
    }
    this.lstn[evname] = fn;
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.SockJSServerStream.prototype.write"></a>[function <span class="apidocSignatureSpan">swarm.SockJSServerStream.prototype.</span>write (data)](#apidoc.element.swarm.SockJSServerStream.prototype.write)
- description and source-code
```javascript
write = function (data) {
    if (this.buf) {
        this.buf.push(data.toString());
    } else {
        this.ws.write(data.toString());
    }
}
```
- example usage
```shell
...
    this.queue = [];
    if (this.id in AsyncLoopbackConnection.pipes) {
        throw new Error('duplicate');
    }
    AsyncLoopbackConnection.pipes[this.id] = this;
    var pair = this.pair();
    if (pair && pair.queue.length) {
        pair.write();
    }
}
AsyncLoopbackConnection.pipes = {};

env.streams.loopback = AsyncLoopbackConnection;

AsyncLoopbackConnection.prototype.pair = function () {
...
```



# <a name="apidoc.module.swarm.Spec"></a>[module swarm.Spec](#apidoc.module.swarm.Spec)

#### <a name="apidoc.element.swarm.Spec.Spec"></a>[function <span class="apidocSignatureSpan">swarm.</span>Spec (str, quant)](#apidoc.element.swarm.Spec.Spec)
- description and source-code
```javascript
function Spec(str, quant) {
    if (str && str.constructor === Spec) {
        str = str.value;
    } else { // later we assume value has valid format
        str = (str || '').toString();
        if (quant && str.charAt(0) >= '0') {
            str = quant + str;
        }
        if (str.replace(Spec.reQTokExt, '')) {
            throw new Error('malformed specifier: ' + str);
        }
    }
    this.value = str;
    this.index = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.Map"></a>[function <span class="apidocSignatureSpan">swarm.Spec.</span>Map (vec)](#apidoc.element.swarm.Spec.Map)
- description and source-code
```javascript
function VersionVectorAsAMap(vec) {
    this.map = {};
    if (vec) {
        this.add(vec);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.as"></a>[function <span class="apidocSignatureSpan">swarm.Spec.</span>as (spec)](#apidoc.element.swarm.Spec.as)
- description and source-code
```javascript
as = function (spec) {
    if (!spec) {
        return new Spec('');
    } else {
        return spec.constructor === Spec ? spec : new Spec(spec);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.base2int"></a>[function <span class="apidocSignatureSpan">swarm.Spec.</span>base2int (base)](#apidoc.element.swarm.Spec.base2int)
- description and source-code
```javascript
base2int = function (base) {
    var ret = 0, l = base.match(Spec.re64l);
    for (var shift = 0; l.length; shift += 6) {
        ret += Spec.base64.indexOf(l.pop()) << shift;
    }
    return ret;
}
```
- example usage
```shell
...
return base + '+' + this.id;
};

LamportClock.prototype.parseTimestamp = function parse (ts) {
var m = ts.match(Spec.reTokExt);
if (!m) {throw new Error('malformed timestamp: '+ts);}
return {
    seq: Spec.base2int(m[1]),
    process: m[2]
};
};

/** Lamport partial order  imperfect semi-logical*/
LamportClock.prototype.checkTimestamp = function see (ts) {
var parsed = this.parseTimestamp(ts);
...
```

#### <a name="apidoc.element.swarm.Spec.int2base"></a>[function <span class="apidocSignatureSpan">swarm.Spec.</span>int2base (i, padlen)](#apidoc.element.swarm.Spec.int2base)
- description and source-code
```javascript
int2base = function (i, padlen) {
    if (i < 0 || i >= (1 << 30)) {
        throw new Error('out of range');
    }
    var ret = '', togo = padlen || 5;
    for (; i || (togo > 0); i >>= 6, togo--) {
        ret = Spec.base64.charAt(i & 63) + ret;
    }
    return ret;
}
```
- example usage
```shell
...
this.seq = 0;
};

LamportClock.prototype.adjustTime = function () {
};

LamportClock.prototype.issueTimestamp = function time () {
var base = Spec.int2base(this.seq++, 5);
return base + '+' + this.id;
};

LamportClock.prototype.parseTimestamp = function parse (ts) {
var m = ts.match(Spec.reTokExt);
if (!m) {throw new Error('malformed timestamp: '+ts);}
return {
...
```

#### <a name="apidoc.element.swarm.Spec.is"></a>[function <span class="apidocSignatureSpan">swarm.Spec.</span>is (str)](#apidoc.element.swarm.Spec.is)
- description and source-code
```javascript
is = function (str) {
    if (str === null || str === undefined) {
        return false;
    }
    return str.constructor === Spec || '' === str.toString().replace(Spec.reQTokExt, '');
}
```
- example usage
```shell
...
    this.emit(spec,value);
};


SharedWebStorage.prototype.installListeners = function () {
    var self = this;
    function onStorageChange(ev) {
        if (Spec.is(ev.key) && ev.newValue) {
            self.onOp(new Spec(ev.key), JSON.parse(ev.newValue));
        }
    }
    window.addEventListener('storage', onStorageChange, false);
};
...
```

#### <a name="apidoc.element.swarm.Spec.parseToken"></a>[function <span class="apidocSignatureSpan">swarm.Spec.</span>parseToken (token_body)](#apidoc.element.swarm.Spec.parseToken)
- description and source-code
```javascript
parseToken = function (token_body) {
    Spec.reTokExt.lastIndex = -1;
    var m = Spec.reTokExt.exec(token_body);
    if (!m) {
        return null;
    }
    return {bare: m[1], ext: m[2] || 'swarm'}; // FIXME not generic
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.pattern"></a>[function <span class="apidocSignatureSpan">swarm.Spec.</span>pattern (spec)](#apidoc.element.swarm.Spec.pattern)
- description and source-code
```javascript
pattern = function (spec) {
    return spec.toString().replace(Spec.reQTokExt, '$1');
}
```
- example usage
```shell
...
// scan/sort specs for existing records
var store = this.store;
var ti;
for (var i = 0; i < store.length; i++) {
    var key = store.key(i);
    if (!Spec.is(key)) { continue; }
    var spec = new Spec(key);
    if (spec.pattern() !== '/#!.') {
        continue; // ops only
    }
    ti = spec.filter('/#');
    var tail = this.tails[ti];
    if (!tail) {
        tail = this.tails[ti] = [];
    }
...
```



# <a name="apidoc.module.swarm.Spec.Map"></a>[module swarm.Spec.Map](#apidoc.module.swarm.Spec.Map)

#### <a name="apidoc.element.swarm.Spec.Map.Map"></a>[function <span class="apidocSignatureSpan">swarm.Spec.</span>Map (vec)](#apidoc.element.swarm.Spec.Map.Map)
- description and source-code
```javascript
function VersionVectorAsAMap(vec) {
    this.map = {};
    if (vec) {
        this.add(vec);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Spec.Map.prototype"></a>[module swarm.Spec.Map.prototype](#apidoc.module.swarm.Spec.Map.prototype)

#### <a name="apidoc.element.swarm.Spec.Map.prototype.add"></a>[function <span class="apidocSignatureSpan">swarm.Spec.Map.prototype.</span>add (versionVector)](#apidoc.element.swarm.Spec.Map.prototype.add)
- description and source-code
```javascript
add = function (versionVector) {
    var vec = new Spec(versionVector, '!'), tok;
    while (undefined !== (tok = vec.token('!'))) {
        var time = tok.bare, source = tok.ext || 'swarm';
        if (time > (this.map[source] || '')) {
            this.map[source] = time;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.Map.prototype.covers"></a>[function <span class="apidocSignatureSpan">swarm.Spec.Map.prototype.</span>covers (version)](#apidoc.element.swarm.Spec.Map.prototype.covers)
- description and source-code
```javascript
covers = function (version) {
    Spec.reTokExt.lastIndex = 0;
    var m = Spec.reTokExt.exec(version);
    var ts = m[1], src = m[2] || 'swarm';
    return ts <= (this.map[src] || '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.Map.prototype.maxTs"></a>[function <span class="apidocSignatureSpan">swarm.Spec.Map.prototype.</span>maxTs ()](#apidoc.element.swarm.Spec.Map.prototype.maxTs)
- description and source-code
```javascript
maxTs = function () {
    var ts = null,
        map = this.map;
    for (var src in map) {
        if (!ts || ts < map[src]) {
            ts = map[src];
        }
    }
    return ts;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.Map.prototype.toString"></a>[function <span class="apidocSignatureSpan">swarm.Spec.Map.prototype.</span>toString (trim)](#apidoc.element.swarm.Spec.Map.prototype.toString)
- description and source-code
```javascript
toString = function (trim) {
    trim = trim || {top: 10, rot: '0'};
    var top = trim.top || 10,
        rot = '!' + (trim.rot || '0'),
        ret = [],
        map = this.map;
    for (var src in map) {
        ret.push('!' + map[src] + (src === 'swarm' ? '' : '+' + src));
    }
    ret.sort().reverse();
    while (ret.length > top || ret[ret.length - 1] <= rot) {
        ret.pop();
    }
    return ret.join('') || '!0';
}
```
- example usage
```shell
...

AsyncLoopbackConnection.prototype.receive = function (string) {
this.lstn.data && this.lstn.data(string);
};

AsyncLoopbackConnection.prototype.write = function (obj) {
var self = this;
obj && self.queue.push(obj.toString());
setTimeout(function () {
    var pair = self.pair();
    if (!pair) {
        return;
    }
    while (self.queue.length) {
        pair.receive(self.queue.shift());
...
```



# <a name="apidoc.module.swarm.Spec.prototype"></a>[module swarm.Spec.prototype](#apidoc.module.swarm.Spec.prototype)

#### <a name="apidoc.element.swarm.Spec.prototype.add"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>add (spec, quant)](#apidoc.element.swarm.Spec.prototype.add)
- description and source-code
```javascript
add = function (spec, quant) {
    if (spec.constructor !== Spec) {
        spec = new Spec(spec, quant);
    }
    return new Spec(this.value + spec.value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.prototype.filter"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>filter (quants)](#apidoc.element.swarm.Spec.prototype.filter)
- description and source-code
```javascript
filter = function (quants) {
    var filterfn = //typeof(quants)==='function' ? quants :
                function (token, quant) {
                    return quants.indexOf(quant) !== -1 ? token : '';
                };
    return new Spec(this.value.replace(Spec.reQTokExt, filterfn));
}
```
- example usage
```shell
...
 *
 * @param {function()} callback
 * @this Set|Vector
 */
onObjectStateReady: function (callback) { // TODO timeout ?
    var self = this;
    function checker() {
        var notInitedYet = self.filter(function (entry) {
            return !entry._version;
        });
        if (!notInitedYet.length) {
            // all entries are inited
            callback();
        } else {
            // wait for some entry not ready yet
...
```

#### <a name="apidoc.element.swarm.Spec.prototype.fits"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>fits (specFilter)](#apidoc.element.swarm.Spec.prototype.fits)
- description and source-code
```javascript
fits = function (specFilter) {
    var myToks = this.value.match(Spec.reQTokExt);
    var filterToks = specFilter.match(Spec.reQTokExt), tok;
    while (tok=filterToks.pop()) {
        if (myToks.indexOf(tok) === -1) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.prototype.get"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>get (quant)](#apidoc.element.swarm.Spec.prototype.get)
- description and source-code
```javascript
function specGet(quant) {
    var i = this.value.indexOf(quant);
    if (i === -1) {
        return '';
    }
    Spec.reQTokExt.lastIndex = i;
    var m = Spec.reQTokExt.exec(this.value);
    return m && m[2];
}
```
- example usage
```shell
...
var swarmHost = new Swarm.Host('unique_client_id');

// 2. connect to your server
swarmHost.connect('ws://localhost:8000/');

// 3.a. create an object
var someMouse = new Mouse();
// OR swarmHost.get('/Mouse');
// OR new Mouse({x:1, y:2});

// 4.a. a locally created object may be touched immediately
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
...
```

#### <a name="apidoc.element.swarm.Spec.prototype.has"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>has (quant)](#apidoc.element.swarm.Spec.prototype.has)
- description and source-code
```javascript
function specHas(quant) {
    if (quant.length===1) {
        return this.value.indexOf(quant) !== -1;
    } else {
        var toks = this.value.match(Spec.reQTokExt);
        return toks.indexOf(quant) !== -1;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.prototype.id"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>id ()](#apidoc.element.swarm.Spec.prototype.id)
- description and source-code
```javascript
id = function () { return this.get('#'); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>isEmpty ()](#apidoc.element.swarm.Spec.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
    return this.value==='';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.prototype.op"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>op ()](#apidoc.element.swarm.Spec.prototype.op)
- description and source-code
```javascript
op = function () { return this.get('.'); }
```
- example usage
```shell
...
    mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
    // this will be triggered by every state change, be it
    // local or remote
    console.log('event: ', spec.op(), val);
    // outputs:
    // set {x:3, y:4}
});
'''

### Creating a simple NodeJS sync server
...
```

#### <a name="apidoc.element.swarm.Spec.prototype.pattern"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>pattern ()](#apidoc.element.swarm.Spec.prototype.pattern)
- description and source-code
```javascript
pattern = function () {
    return Spec.pattern(this.value);
}
```
- example usage
```shell
...
// scan/sort specs for existing records
var store = this.store;
var ti;
for (var i = 0; i < store.length; i++) {
    var key = store.key(i);
    if (!Spec.is(key)) { continue; }
    var spec = new Spec(key);
    if (spec.pattern() !== '/#!.') {
        continue; // ops only
    }
    ti = spec.filter('/#');
    var tail = this.tails[ti];
    if (!tail) {
        tail = this.tails[ti] = [];
    }
...
```

#### <a name="apidoc.element.swarm.Spec.prototype.set"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>set (spec, quant)](#apidoc.element.swarm.Spec.prototype.set)
- description and source-code
```javascript
function specSet(spec, quant) {
    var ret = new Spec(spec, quant);
    var m;
    Spec.reQTokExt.lastIndex = 0;
    while (null !== (m = Spec.reQTokExt.exec(this.value))) {
        if (!ret.has(m[1])) {
            ret = ret.add(m[0]);
        }
    }
    return ret.sort();
}
```
- example usage
```shell
...

// 3.a. create an object
var someMouse = new Mouse();
// OR swarmHost.get('/Mouse');
// OR new Mouse({x:1, y:2});

// 4.a. a locally created object may be touched immediately
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
...
```

#### <a name="apidoc.element.swarm.Spec.prototype.sort"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>sort ()](#apidoc.element.swarm.Spec.prototype.sort)
- description and source-code
```javascript
sort = function () {
    function Q(a, b) {
        var qa = a.charAt(0), qb = b.charAt(0), q = Spec.quants;
        return (q.indexOf(qa) - q.indexOf(qb)) || (a < b);
    }

    var split = this.value.match(Spec.reQTokExt);
    return new Spec(split ? split.sort(Q).join('') : '');
}
```
- example usage
```shell
...
    var tail = this.tails[ti];
    if (!tail) {
        tail = this.tails[ti] = [];
    }
    tail.push(spec.filter('!.'));
}
for (ti in this.tails) {
    this.tails[ti].sort();
}
};


SharedWebStorage.prototype.writeOp = function wsOp(spec, value, src) {
var ti = spec.filter('/#');
var vm = spec.filter('!.');
...
```

#### <a name="apidoc.element.swarm.Spec.prototype.source"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>source ()](#apidoc.element.swarm.Spec.prototype.source)
- description and source-code
```javascript
source = function () { return this.token('!').ext; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.prototype.toString"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>toString ()](#apidoc.element.swarm.Spec.prototype.toString)
- description and source-code
```javascript
toString = function () { return this.value; }
```
- example usage
```shell
...

AsyncLoopbackConnection.prototype.receive = function (string) {
this.lstn.data && this.lstn.data(string);
};

AsyncLoopbackConnection.prototype.write = function (obj) {
var self = this;
obj && self.queue.push(obj.toString());
setTimeout(function () {
    var pair = self.pair();
    if (!pair) {
        return;
    }
    while (self.queue.length) {
        pair.receive(self.queue.shift());
...
```

#### <a name="apidoc.element.swarm.Spec.prototype.tok"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>tok (quant)](#apidoc.element.swarm.Spec.prototype.tok)
- description and source-code
```javascript
function specGet(quant) {
    var i = this.value.indexOf(quant);
    if (i === -1) { return ''; }
    Spec.reQTokExt.lastIndex = i;
    var m = Spec.reQTokExt.exec(this.value);
    return m && m[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.prototype.token"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>token (quant)](#apidoc.element.swarm.Spec.prototype.token)
- description and source-code
```javascript
token = function (quant) {
    var at = quant ? this.value.indexOf(quant, this.index) : this.index;
    if (at === -1) {
        return undefined;
    }
    Spec.reQTokExt.lastIndex = at;
    var m = Spec.reQTokExt.exec(this.value);
    this.index = Spec.reQTokExt.lastIndex;
    if (!m) {
        return undefined;
    }
    return {quant: m[1], body: m[2], bare: m[3], ext: m[4]};
}
```
- example usage
```shell
...
    state: function (spec, text, src) {
        console.log('what?');
    }
},
ops: {
    insert: function (spec, ins, src) {
        var w1 = [], w4 = [];
        var vt = spec.token('!'), v = vt.bare;
        var ts = v.substr(0, 5), seq = v.substr(5) || '00';
        var seqi = Spec.base2int(seq);
        for (var i = 0; i < this.weave.length; i++) {
            var id = this.ids[i];
            w1.push(this.weave.charAt(i));
            w4.push(id);
            if (id in ins) {
...
```

#### <a name="apidoc.element.swarm.Spec.prototype.type"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>type ()](#apidoc.element.swarm.Spec.prototype.type)
- description and source-code
```javascript
type = function () { return this.get('/'); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.prototype.typeid"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>typeid ()](#apidoc.element.swarm.Spec.prototype.typeid)
- description and source-code
```javascript
typeid = function () { return this.filter('/#'); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Spec.prototype.version"></a>[function <span class="apidocSignatureSpan">swarm.Spec.prototype.</span>version ()](#apidoc.element.swarm.Spec.prototype.version)
- description and source-code
```javascript
version = function () { return this.get('!'); }
```
- example usage
```shell
...
    }
    this.weave = w1.join('');
    this.ids = w4;
    this.rebuild();
},
remove: function (spec, rm, src) {
    var w1 = [], w4 = [];
    var v = spec.version();
    for (var i = 0; i < this.weave.length; i++) {
        w1.push(this.weave.charAt(i));
        w4.push(this.ids[i]);
        if (this.ids[i] in rm) {
            w1.push('\u0008');
            w4.push(v);
        }
...
```



# <a name="apidoc.module.swarm.Storage"></a>[module swarm.Storage](#apidoc.module.swarm.Storage)

#### <a name="apidoc.element.swarm.Storage.Storage"></a>[function <span class="apidocSignatureSpan">swarm.</span>Storage (async)](#apidoc.element.swarm.Storage.Storage)
- description and source-code
```javascript
function Storage(async) {
    this.async = !!async || false;
    this.states = {};
    this.tails = {};
    this.counts = {};
    this._host = null;
    // many implementations do not push changes
    // so there are no listeners
    this.lstn = null;
    this._id = 'some_storage';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Storage.prototype"></a>[module swarm.Storage.prototype](#apidoc.module.swarm.Storage.prototype)

#### <a name="apidoc.element.swarm.Storage.prototype.anyOp"></a>[function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>anyOp (spec, value, src)](#apidoc.element.swarm.Storage.prototype.anyOp)
- description and source-code
```javascript
anyOp = function (spec, value, src) {
    var self = this;
    var ti = spec.filter('/#');
    this.writeOp(spec, value, function (err) {
        if (err) {
            this.close(err); // the log is sacred
        }
    });
    self.counts[ti] = self.counts[ti] || 0;
    if (++self.counts[ti]>self.MAX_LOG_SIZE) {
        // The storage piggybacks on the object's state/log handling logic
        // First, it adds an op to the log tail unless the log is too long...
        // ...otherwise it sends back a subscription effectively requesting
        // the state, on state arrival zeroes the tail.
        delete self.counts[ti];
        src.deliver(spec.set('.reon'), '!0.init', self);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Storage.prototype.close"></a>[function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>close (callback)](#apidoc.element.swarm.Storage.prototype.close)
- description and source-code
```javascript
close = function (callback) {
    if (callback) { callback(); }
}
```
- example usage
```shell
...
        }
    }, 1);
};

AsyncLoopbackConnection.prototype.close = function () {
    delete AsyncLoopbackConnection.pipes[this.id];
    var pair = this.pair();
    pair && pair.close();
    this.lstn.close && this.lstn.close();
};
...
```

#### <a name="apidoc.element.swarm.Storage.prototype.deliver"></a>[function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>deliver (spec, value, src)](#apidoc.element.swarm.Storage.prototype.deliver)
- description and source-code
```javascript
deliver = function (spec, value, src) {
    var ret;
    switch (spec.op()) {
        // A storage is always an "uplink" so it never receives reon, reoff.
    case 'on':
        ret = this.on(spec, value, src); break;
    case 'off':
        ret = this.off(spec, value, src); break;
    case 'init':
        if (value._version) { // state
            ret = this.init(spec, value, src);
        } else { // patch
            var ti = spec.filter('/#');
            var specs = [], s;
            for(s in value._tail) {  specs.push(s);  }
            specs.sort();
            while (s=specs.pop()) {
                ret = this.anyOp( ti.add(s), value._tail[s], src);
            }
        }
        break;
    default:
        ret = this.anyOp(spec, value, src);
    }
    return ret;
}
```
- example usage
```shell
...
if (this.callbacks===null) { return; }
var that = this.owner || src;
for(var i=0; i<this.callbacks.length; i++) {
    var cb = this.callbacks[i];
    if (cb.constructor===Function) {
        cb.call(that,spec,value,src);
    } else {
        cb.deliver(spec,value,src);
    }
}
};

ProxyListener.prototype.on = function (callback) {
if (this.callbacks===null) { this.callbacks = []; }
this.callbacks.push(callback);
...
```

#### <a name="apidoc.element.swarm.Storage.prototype.emit"></a>[function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>emit (spec, value)](#apidoc.element.swarm.Storage.prototype.emit)
- description and source-code
```javascript
emit = function (spec, value) {
    var ti = spec.filter('/#');
    var ln = this.lstn[ti];
    if (!ln) {return;}
    if (ln && ln.constructor===Array) {
        for(var i=0; ln && i<ln.length; i++) {
            var l = ln[i];
            if (l && l.constructor===Function) {
                l(spec,value,this);
            } else if (l && l.deliver) {
                l.deliver(spec,value,this);
            }
        }
    } else if (ln && ln.deliver) {
        ln.deliver(spec,value,this);
    } else if (ln && ln.constructor===Function) {
        ln(spec,value,this);
    }
}
```
- example usage
```shell
...
var tail = this.tails[ti];
if (!tail) {
    tail = this.tails[ti] = [];
} else if (tail.indexOf(vo)!==-1) {
    return; // replay
}
tail.push(vo);
this.emit(spec,value);
};


SharedWebStorage.prototype.installListeners = function () {
var self = this;
function onStorageChange(ev) {
    if (Spec.is(ev.key) && ev.newValue) {
...
```

#### <a name="apidoc.element.swarm.Storage.prototype.init"></a>[function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>init (spec, state, src)](#apidoc.element.swarm.Storage.prototype.init)
- description and source-code
```javascript
init = function (spec, state, src) {
    var ti = spec.filter('/#'), self=this;
    var saveops = this.tails[ti];
    this.writeState(spec, state, function (err) {
        if (err) {
            console.error('state dump error:', err);
        } else {
            var tail = self.tails[ti] || (self.tails[ti] = {});
            for(var op in saveops) { // OK, let's keep that in the log
                tail[op] = saveops[op];
            }
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Storage.prototype.off"></a>[function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>off (spec, value, src)](#apidoc.element.swarm.Storage.prototype.off)
- description and source-code
```javascript
off = function (spec, value, src) {
    if (!this.lstn) {
        return;
    }
    var ti = spec.filter('/#');
    var ls = this.lstn[ti];
    if (ls === src) {
        delete this.lstn[ti];
    } else if (ls && ls.constructor === Array) {
        var cleared = ls.filter(function (v) {return v !== src;});
        if (cleared.length) {
            this.lstn[ti] = cleared;
        } else {
            delete this.lstn[ti];
        }
    }
}
```
- example usage
```shell
...

/**
 * Unsubscribe from collections entries' events
 * @param {function(*)} callback
 * @this Set|Vector
 */
offObjectEvent: function (callback) {
    this._proxy.off(callback);
},

/**
 * Waits for collection to receive state from cache or uplink and then invokes passed callback
 *
 * @param {function()} callback
 * @this Set|Vector
...
```

#### <a name="apidoc.element.swarm.Storage.prototype.on"></a>[function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>on (spec, base, src)](#apidoc.element.swarm.Storage.prototype.on)
- description and source-code
```javascript
function storageOn(spec, base, src) {
    var ti = spec.filter('/#');

    if (this.lstn) {
        var ls = this.lstn[ti];
        if (ls === undefined) {
            ls = src;
        } else if (ls !== src) {
            if (ls.constructor !== Array) {
                ls = [ls];
            }
            ls.push(src);
        }
        this.lstn[ti] = ls;
    }

    var self = this;
    var state;
    var tail;

    function sendResponse() {
        if (!state) {
            if (self.isRoot) {// && !spec.token('#').ext) {
                // make 0 state for a global object TODO move to Host
                state = {_version: '!0'};
            }
        }
        if (tail) {
            if (!state) {state={};}
            state._tail = state._tail || {};
            for (var s in tail) {
                state._tail[s] = tail[s];
            }
        }
        var tiv = ti.add(spec.version(), '!');
        if (state) {
            src.deliver(tiv.add('.init'), state, self);
            src.deliver(tiv.add('.reon'), Syncable.stateVersionVector(state), self); // TODO and the tail
        } else {
            src.deliver(tiv.add('.reon'), '!0', self); // state unknown
        }
    }

    this.readState(ti, function (err, s) {
        state = s || null;
        if (tail !== undefined) {
            sendResponse();
        }
    });

    this.readOps(ti, function (err, t) {
        tail = t || null;
        if (state !== undefined) {
            sendResponse();
        }
    });
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.Storage.prototype.readOps"></a>[function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>readOps (ti, callback)](#apidoc.element.swarm.Storage.prototype.readOps)
- description and source-code
```javascript
readOps = function (ti, callback) {
    var tail = JSON.parse(this.tails[ti] || null);
    callback(null, tail);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Storage.prototype.readState"></a>[function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>readState (ti, callback)](#apidoc.element.swarm.Storage.prototype.readState)
- description and source-code
```javascript
readState = function (ti, callback) {
    var state = JSON.parse(this.states[ti] || null);

    function sendResponse() {
        callback(null, state);
    }

    // may force async behavior
    this.async ? setTimeout(sendResponse, 1) : sendResponse();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Storage.prototype.writeOp"></a>[function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>writeOp (spec, value, cb)](#apidoc.element.swarm.Storage.prototype.writeOp)
- description and source-code
```javascript
writeOp = function (spec, value, cb) {
    var ti = spec.filter('/#');
    var vm = spec.filter('!.');
    var tail = this.tails[ti] || (this.tails[ti] = {});
    if (tail[vm]) {
        console.error('op replay @storage'+vm+new Error().stack);
    }
    tail[vm] = JSON.stringify(value);
    cb();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Storage.prototype.writeState"></a>[function <span class="apidocSignatureSpan">swarm.Storage.prototype.</span>writeState (spec, state, cb)](#apidoc.element.swarm.Storage.prototype.writeState)
- description and source-code
```javascript
writeState = function (spec, state, cb) {
    var ti = spec.filter('/#');
    this.states[ti] = JSON.stringify(state);
    // tail is zeroed on state flush
    delete this.tails[ti];
    // callback is mandatory
    cb();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Syncable"></a>[module swarm.Syncable](#apidoc.module.swarm.Syncable)

#### <a name="apidoc.element.swarm.Syncable.Syncable"></a>[function <span class="apidocSignatureSpan">swarm.</span>Syncable ()](#apidoc.element.swarm.Syncable.Syncable)
- description and source-code
```javascript
function Syncable() {
    // listeners represented as objects that have deliver() method
    this._lstn = [',']; // we unshift() uplink listeners and push() downlinks
    // ...so _lstn is like [server1, server2, storage, ',', view, listener]
    // The most correct way to specify a version is the version vector,
    // but that one may consume more space than the data itself in some cases.
    // Hence, _version is not a fully specified version vector (see version()
    // instead). _version is essentially is the greatest operation timestamp
    // (Lamport-like, i.e. "time+source"), sometimes amended with additional
    // timestamps. Its main features:
    // (1) changes once the object's state changes
    // (2) does it monotonically (in the alphanum order sense)
    this._version = '';
    // make sense of arguments
    var args = Array.prototype.slice.call(arguments);
    this._host = (args.length && args[args.length - 1]._type === 'Host') ?
            args.pop() : env.localhost;
    if (Spec.is(args[0])) {
        this._id = new Spec(args.shift()).id() || this._host.time();
    } else if (typeof(args[0]) === 'string') {
        this._id = args.shift(); // TODO format
    } else {
        this._id = this._host.time();
        this._version = '!0'; // may apply state in the constructor, see Model
    }
    //var state = args.length ? args.pop() : (fresh?{}:undefined);
    // register with the host
    var doubl = this._host.register(this);
    if (doubl !== this) { return doubl; }
    // locally created objects get state immediately
    // (while external-id objects need to query uplinks)
<span class="apidocCodeCommentSpan">    /*if (fresh && state) {
     state._version = '!'+this._id;
     var pspec = this.spec().add(state._version).add('.init');
     this.deliver(pspec,state,this._host);
     }*/
</span>    this.reset();
    // find uplinks, subscribe
    this.checkUplink();
    // TODO inplement state push
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable._super"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.</span>_super ()](#apidoc.element.swarm.Syncable._super)
- description and source-code
```javascript
function Syncable() {
    // listeners represented as objects that have deliver() method
    this._lstn = [',']; // we unshift() uplink listeners and push() downlinks
    // ...so _lstn is like [server1, server2, storage, ',', view, listener]
    // The most correct way to specify a version is the version vector,
    // but that one may consume more space than the data itself in some cases.
    // Hence, _version is not a fully specified version vector (see version()
    // instead). _version is essentially is the greatest operation timestamp
    // (Lamport-like, i.e. "time+source"), sometimes amended with additional
    // timestamps. Its main features:
    // (1) changes once the object's state changes
    // (2) does it monotonically (in the alphanum order sense)
    this._version = '';
    // make sense of arguments
    var args = Array.prototype.slice.call(arguments);
    this._host = (args.length && args[args.length - 1]._type === 'Host') ?
            args.pop() : env.localhost;
    if (Spec.is(args[0])) {
        this._id = new Spec(args.shift()).id() || this._host.time();
    } else if (typeof(args[0]) === 'string') {
        this._id = args.shift(); // TODO format
    } else {
        this._id = this._host.time();
        this._version = '!0'; // may apply state in the constructor, see Model
    }
    //var state = args.length ? args.pop() : (fresh?{}:undefined);
    // register with the host
    var doubl = this._host.register(this);
    if (doubl !== this) { return doubl; }
    // locally created objects get state immediately
    // (while external-id objects need to query uplinks)
<span class="apidocCodeCommentSpan">    /*if (fresh && state) {
     state._version = '!'+this._id;
     var pspec = this.spec().add(state._version).add('.init');
     this.deliver(pspec,state,this._host);
     }*/
</span>    this.reset();
    // find uplinks, subscribe
    this.checkUplink();
    // TODO inplement state push
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.addReaction"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.</span>addReaction (op, fn)](#apidoc.element.swarm.Syncable.addReaction)
- description and source-code
```javascript
addReaction = function (op, fn) {
    var reactions = this.prototype._reactions;
    var list = reactions[op];
    list || (list = reactions[op] = []);
    list.push(fn);
    return {op: op, fn: fn};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.extend"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.</span>extend (fn, own)](#apidoc.element.swarm.Syncable.extend)
- description and source-code
```javascript
extend = function (fn, own) {
    var parent = this, fnid;
    if (fn.constructor !== Function) {
        var id = fn.toString();
        fn = function SomeSyncable() {
            return parent.apply(this, arguments);
        };
        fnid = id; // if only it worked
    } else { // please call Syncable.constructor.apply(this,args) in your constructor
        fnid = fnname(fn);
    }

    // inheritance trick from backbone.js
    var SyncProto = function () {
        this.constructor = fn;
        this._neutrals = {};
        this._ops = {};
        this._reactions = {};

        var event,
            name;
        if (parent._pt) {
            //copy _neutrals & _ops from parent
            for (event in parent._pt._neutrals) {
                this._neutrals[event] = parent._pt._neutrals[event];
            }
            for (event in parent._pt._ops) {
                this._ops[event] = parent._pt._ops[event];
            }
        }

        // "Methods" are serialized, logged and delivered to replicas
        for (name in own.ops || {}) {
            if (Syncable.reMethodName.test(name)) {
                this._ops[name] = own.ops[name];
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid op name:',name);
            }
        }

        // "Neutrals" don't change the state
        for (name in own.neutrals || {}) {
            if (Syncable.reMethodName.test(name)) {
                this._neutrals[name] = own.neutrals[name];
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid neutral op name:',name);
            }
        }

        // "Remotes" are serialized and sent upstream (like RPC calls)
        for (name in own.remotes || {}) {
            if (Syncable.reMethodName.test(name)) {
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid rpc name:',name);
            }
        }

        // add mixins
        (own.mixins || []).forEach(function (mixin) {
            for (var name in mixin) {
                this[name] = mixin[name];
            }
        }, this);

        // add other members
        for (name in own) {
            if (Syncable.reMethodName.test(name)) {
                var memberType = own[name].constructor;
                if (memberType === Function) { // non-op method
                    // these must change state ONLY by invoking ops
                    this[name] = own[name];
                } else if (memberType===String || memberType===Number) {
                    this[name] = own[name]; // some static constant, OK
                } else if (name in Syncable.memberClasses) {
                    // see above
                    continue;
                } else {
                    console.warn('invalid member:',name,memberType);
                }
            } else {
                console.warn('invalid member name:',name);
            }
        }

        // add reactions
        for (name in own.reactions || {}) {
            var reaction = own.reactions[name];
            if (!reaction) { continue; }

            switch (typeof reaction) {
            case 'function':
                // handler-function
                this._reactions[name] = [reaction];
                break;
            case 'string':
                // handler-method name
                this._reactions[name] = [this[name]];
                break;
            default:
                if (reaction.constructor === Array) {
                    // array of handlers
                    this._reactions[name] = reaction.map(function (item) {
                        switch (typeof item) {
                        case 'function':
                            return item;
                        case 'string':
                            return this[item];
                        default:
                            throw new Error('unexpected reaction type');
                        }
                    }, this);
                } else {
                    throw new Error('unex ...
```
- example usage
```shell
...
these demos are normally online at http://ppyr.us and http://ppyr.us:8001/demo3/index.html respectively.

### Creating your first simple synchronized type

'''js
var Swarm = require('swarm');

var Mouse = Swarm.Model.extend('Mouse', {
    defaults: {
        name: 'Mickey',
        x: 0,
        y: 0
    }
});
...
```

#### <a name="apidoc.element.swarm.Syncable.isOpSink"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.</span>isOpSink (obj)](#apidoc.element.swarm.Syncable.isOpSink)
- description and source-code
```javascript
isOpSink = function (obj) {
    if (!obj) { return false; }
    if (obj.constructor === Function) { return true; }
    if (obj.deliver && obj.deliver.constructor === Function) { return true; }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.listenerEquals"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.</span>listenerEquals (ln, other)](#apidoc.element.swarm.Syncable.listenerEquals)
- description and source-code
```javascript
listenerEquals = function (ln, other) {
    return !!ln && ((ln === other) ||
        (ln._src && ln._src === other) ||
        (ln.fn && ln.fn === other) ||
        (ln.sink && ln.sink === other));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.removeReaction"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.</span>removeReaction (handle)](#apidoc.element.swarm.Syncable.removeReaction)
- description and source-code
```javascript
removeReaction = function (handle) {
    var op = handle.op,
        fn = handle.fn,
        list = this.prototype._reactions[op],
        i = list.indexOf(fn);
    if (i === -1) {
        throw new Error('reaction unknown');
    }
    list[i] = undefined; // such a peculiar pattern not to mess up out-of-callback removal
    while (list.length && !list[list.length - 1]) {
        list.pop();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.stateVersionVector"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.</span>stateVersionVector (state)](#apidoc.element.swarm.Syncable.stateVersionVector)
- description and source-code
```javascript
function stateVersionVector(state) {
    var op,
        map = new Spec.Map( (state._version||'!0') + (state._vector || '') );
    if (state._oplog) {
        for (op in state._oplog) {
            map.add(op);
        }
    }
    if (state._tail) {
        for (op in state._tail) {
            map.add(op);
        }
    }
    return map.toString();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Syncable.prototype"></a>[module swarm.Syncable.prototype](#apidoc.module.swarm.Syncable.prototype)

#### <a name="apidoc.element.swarm.Syncable.prototype.acl"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>acl (spec, val, src)](#apidoc.element.swarm.Syncable.prototype.acl)
- description and source-code
```javascript
acl = function (spec, val, src) {
    return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.apply"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>apply (values)](#apidoc.element.swarm.Syncable.prototype.apply)
- description and source-code
```javascript
apply = function (values) {
    for (var key in values) {
        if (Syncable.reFieldName.test(key)) { // skip special fields
            var def = this.constructor.defaults[key];
            this[key] = def && def.type ?
                new def.type(values[key]) : values[key];
        }
    }
}
```
- example usage
```shell
...
}

WebSocketStream.prototype.on = function (evname, fn) {
    if (evname in this.lstn) {
        var self = this,
            prev_fn = this.lstn[evname];
        this.lstn[evname] = function () {
            prev_fn.apply(self, arguments);
            fn.apply(self, arguments);
        };
    } else {
        this.lstn[evname] = fn;
    }
};
...
```

#### <a name="apidoc.element.swarm.Syncable.prototype.callReactions"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>callReactions (spec, value, src)](#apidoc.element.swarm.Syncable.prototype.callReactions)
- description and source-code
```javascript
callReactions = function (spec, value, src) {
    var superReactions = syncProto._super.callReactions;
    if ('function' === typeof superReactions) {
        superReactions.call(this, spec, value, src);
    }
    var r = syncProto._reactions[spec.op()];
    if (r) {
        r.constructor !== Array && (r = [r]);
        for (var i = 0; i < r.length; i++) {
            r[i] && r[i].call(this, spec, value, src);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.checkUplink"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>checkUplink ()](#apidoc.element.swarm.Syncable.prototype.checkUplink)
- description and source-code
```javascript
checkUplink = function () {
    var new_uplinks = this._host.getSources(this.spec()).slice(),
        up, self = this;
    // the plan is to eliminate extra subscriptions and to
    // establish missing ones; that only affects outbound subs
    for (var i = 0; i < this._lstn.length && this._lstn[i] != ','; i++) {
        up = this._lstn[i];
        if (!up) {
            continue;
        }
        up._src && (up = up._src); // unready
        var up_idx = new_uplinks.indexOf(up);
        if (up_idx === -1) { // don't need this uplink anymore
            up.deliver(this.newEventSpec('off'), '', this);
        } else {
            new_uplinks[up_idx] = undefined;
        }
    }
    // subscribe to the new
    for (i = 0; i < new_uplinks.length; i++) {
        up = new_uplinks[i];
        if (!up) {
            continue;
        }
        var onspec = this.newEventSpec('on');
        this._lstn.unshift({
            _op: 'reon',
            _src: up,
            deliver: function (spec, base, src) {
                if (spec.version() !== onspec.version()) {
                    return;
                } // not mine

                var i = self.getListenerIndex(this);
                self._lstn[i] = up;
            }
        });
        up.deliver(onspec, this.version().toString(), this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.close"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>close ()](#apidoc.element.swarm.Syncable.prototype.close)
- description and source-code
```javascript
close = function () {
    var l = this._lstn,
        s = this.spec(),
        uplink;

    this._id = null; // no id - no object; prevent relinking
    while ((uplink = l.shift()) && uplink !== ',') {
        uplink.off(s, null, this);
    }
    while (l.length) {
        l.pop().deliver(s.set('.reoff'), null, this);
    }
    this._host.unregister(this);
}
```
- example usage
```shell
...
        }
    }, 1);
};

AsyncLoopbackConnection.prototype.close = function () {
    delete AsyncLoopbackConnection.pipes[this.id];
    var pair = this.pair();
    pair && pair.close();
    this.lstn.close && this.lstn.close();
};
...
```

#### <a name="apidoc.element.swarm.Syncable.prototype.constructor"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>constructor ()](#apidoc.element.swarm.Syncable.prototype.constructor)
- description and source-code
```javascript
function Syncable() {
    // listeners represented as objects that have deliver() method
    this._lstn = [',']; // we unshift() uplink listeners and push() downlinks
    // ...so _lstn is like [server1, server2, storage, ',', view, listener]
    // The most correct way to specify a version is the version vector,
    // but that one may consume more space than the data itself in some cases.
    // Hence, _version is not a fully specified version vector (see version()
    // instead). _version is essentially is the greatest operation timestamp
    // (Lamport-like, i.e. "time+source"), sometimes amended with additional
    // timestamps. Its main features:
    // (1) changes once the object's state changes
    // (2) does it monotonically (in the alphanum order sense)
    this._version = '';
    // make sense of arguments
    var args = Array.prototype.slice.call(arguments);
    this._host = (args.length && args[args.length - 1]._type === 'Host') ?
            args.pop() : env.localhost;
    if (Spec.is(args[0])) {
        this._id = new Spec(args.shift()).id() || this._host.time();
    } else if (typeof(args[0]) === 'string') {
        this._id = args.shift(); // TODO format
    } else {
        this._id = this._host.time();
        this._version = '!0'; // may apply state in the constructor, see Model
    }
    //var state = args.length ? args.pop() : (fresh?{}:undefined);
    // register with the host
    var doubl = this._host.register(this);
    if (doubl !== this) { return doubl; }
    // locally created objects get state immediately
    // (while external-id objects need to query uplinks)
<span class="apidocCodeCommentSpan">    /*if (fresh && state) {
     state._version = '!'+this._id;
     var pspec = this.spec().add(state._version).add('.init');
     this.deliver(pspec,state,this._host);
     }*/
</span>    this.reset();
    // find uplinks, subscribe
    this.checkUplink();
    // TODO inplement state push
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.deliver"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>deliver (spec, value, lstn)](#apidoc.element.swarm.Syncable.prototype.deliver)
- description and source-code
```javascript
deliver = function (spec, value, lstn) {
    spec = Spec.as(spec);
    var opver = '!' + spec.version();
    var error;

    function fail(msg, ex) {
        console.error(msg, spec, value, (ex && ex.stack) || ex || new Error(msg));
        if (typeof(lstn) === 'function') {
            lstn(spec.set('.fail'), msg);
        } else if (lstn && typeof(lstn.error) === 'function') {
            lstn.error(spec, msg);
        } // else { } no callback provided
    }

    // sanity checks
    if (spec.pattern() !== '/#!.') {
        return fail('malformed spec', spec);
    }
    if (!this._id) {
        return fail('undead object invoked');
    }
    if (error = this.validate(spec, value)) {
        return fail('invalid input, ' + error, value);
    }
    if (!this.acl(spec, value, lstn)) {
        return fail('access violation', spec);
    }

    env.debug && env.log(spec, value, lstn);

    try {
        var call = spec.op();
        if (this._ops[call]) {  // FIXME name=>impl table
            if (this.isReplay(spec)) { // it happens
                console.warn('replay', spec);
                return;
            }
            // invoke the implementation
            this._ops[call].call(this, spec, value, lstn); // NOTE: no return value
            // once applied, may remember in the log...
            if (spec.op() !== 'init') {
                this._oplog && (this._oplog[spec.filter('!.')] = value);
                // this._version is practically a label that lets you know whether
                // the state has changed. Also, it allows to detect some cases of
                // concurrent change, as it is always set to the maximum version id
                // received by this object. Still, only the full version vector may
                // precisely and uniquely specify the current version (see version()).
                this._version = (opver > this._version) ? opver : this._version + opver;
            } else {
                value = this.diff('!0');
            }
            // ...and relay further to downstream replicas and various listeners
            this.emit(spec, value, lstn);
        } else if (this._neutrals[call]) {
            // invoke the implementation
            this._neutrals[call].call(this, spec, value, lstn);
            // and relay to listeners
            this.emit(spec, value, lstn);
        } else {
            this.unimplemented(spec, value, lstn);
        }
    } catch (ex) { // log and rethrow; don't relay further; don't log
        return fail("method execution failed", ex);
    }

    // to force async signatures we eat the returned value silently
    return spec;
}
```
- example usage
```shell
...
if (this.callbacks===null) { return; }
var that = this.owner || src;
for(var i=0; i<this.callbacks.length; i++) {
    var cb = this.callbacks[i];
    if (cb.constructor===Function) {
        cb.call(that,spec,value,src);
    } else {
        cb.deliver(spec,value,src);
    }
}
};

ProxyListener.prototype.on = function (callback) {
if (this.callbacks===null) { this.callbacks = []; }
this.callbacks.push(callback);
...
```

#### <a name="apidoc.element.swarm.Syncable.prototype.diff"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>diff (base)](#apidoc.element.swarm.Syncable.prototype.diff)
- description and source-code
```javascript
diff = function (base) {
    //var vid = new Spec(this._version).get('!'); // first !token
    //var spec = vid + '.patch';
    if (!this._version) { return undefined; }
    this.distillLog(); // TODO optimize?
    var patch, spec;
    if (base && base != '!0' && base != '0') { // FIXME ugly
        var map = new Spec.Map(base || '');
        for (spec in this._oplog) {
            if (!map.covers(new Spec(spec).version())) {
                patch = patch || {_tail: {}}; // NOTE: no _version
                patch._tail[spec] = this._oplog[spec];
            }
        }
    } else {
        patch = {_version: '!0', _tail: {}}; // zero state plus the tail
        for (spec in this._oplog) {
            patch._tail[spec] = this._oplog[spec];
        }
    }
    return patch;
}
```
- example usage
```shell
...
 pos += m[0].length;
 }

 this.tids = tids;*/
this.text = this.weave.replace(/[^\u0008][\u0008]+/mg, '').substr(1);
    },
    set: function (newText) {
var patch = Text.diff(this.text, newText);
var rm = null, ins = null, weave = this.weave;
var re_atom = /[^\u0008]([^\u0008][\u0008]+)*/mg;
var atom;

function skip(n) {
    for (n = n || 1; n > 0; n--) {
        atom = re_atom.exec(weave);
...
```

#### <a name="apidoc.element.swarm.Syncable.prototype.distillLog"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>distillLog ()](#apidoc.element.swarm.Syncable.prototype.distillLog)
- description and source-code
```javascript
distillLog = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.emit"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>emit (spec, value, src)](#apidoc.element.swarm.Syncable.prototype.emit)
- description and source-code
```javascript
emit = function (spec, value, src) {
    var ls = this._lstn,
        op = spec.op(),
        is_neutrals = op in this._neutrals;
    if (ls) {
        var notify = [];
        for (var i = 0; i < ls.length; i++) {
            var l = ls[i];
            // skip empties, deferreds and the source
            if (!l || l === ',' || l === src) { continue; }
            if (is_neutrals && l._op !== op) { continue; }
            if (l._op && l._op !== op) { continue; }
            notify.push(l);
        }
        for (i = 0; i < notify.length; i++) { // screw it I want my 'this'
            try {
                notify[i].deliver(spec, value, this);
            } catch (ex) {
                console.error(ex.message, ex.stack);
            }
        }
    }
    this.callReactions(spec, value, src);
}
```
- example usage
```shell
...
var tail = this.tails[ti];
if (!tail) {
    tail = this.tails[ti] = [];
} else if (tail.indexOf(vo)!==-1) {
    return; // replay
}
tail.push(vo);
this.emit(spec,value);
};


SharedWebStorage.prototype.installListeners = function () {
var self = this;
function onStorageChange(ev) {
    if (Spec.is(ev.key) && ev.newValue) {
...
```

#### <a name="apidoc.element.swarm.Syncable.prototype.error"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>error ()](#apidoc.element.swarm.Syncable.prototype.error)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
...
        this.buf = buf; //will wait for "open"
    }
    ws.on('close', function () { ln.close && ln.close(); });
    ws.on('data', function (msg) {
        try {
            ln.data && ln.data(msg);
        } catch (ex) {
            console.error('message processing fails', ex);
            ln.error && ln.error(ex.message);
        }
    });
}

module.exports = SockJSStream;
...
```

#### <a name="apidoc.element.swarm.Syncable.prototype.gc"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>gc ()](#apidoc.element.swarm.Syncable.prototype.gc)
- description and source-code
```javascript
gc = function () {
    var l = this._lstn;
    if (!l.length || (l.length === 1 && !l[0])) {
        this.close();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.getListenerIndex"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>getListenerIndex (search_for, uplinks_only)](#apidoc.element.swarm.Syncable.prototype.getListenerIndex)
- description and source-code
```javascript
getListenerIndex = function (search_for, uplinks_only) {
    var i = this._lstn.indexOf(search_for),
        l;
    if (i > -1) { return i; }

    for (i = 0, l = this._lstn.length; i < l; i++) {
        var ln = this._lstn[i];
        if (uplinks_only && ln === ',') {
            return -1;
        }
        if (Syncable.listenerEquals(ln, search_for)) {
            return i;
        }
    }
    return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.hasState"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>hasState ()](#apidoc.element.swarm.Syncable.prototype.hasState)
- description and source-code
```javascript
hasState = function () {
    return !!this._version;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.init"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>init ()](#apidoc.element.swarm.Syncable.prototype.init)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.isReplay"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>isReplay (spec)](#apidoc.element.swarm.Syncable.prototype.isReplay)
- description and source-code
```javascript
isReplay = function (spec) {
    if (!this._version) { return false; }
    if (spec.op() === 'init') { return false; } // these are .on !vids
    var opver = spec.version();
    if (opver > this._version.substr(1)) { return false; }
    if (spec.filter('!.').toString() in this._oplog) { return true; }// TODO log trimming, vvectors?
    return this.version().covers(opver); // heavyweight
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.newEventSpec"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>newEventSpec (op)](#apidoc.element.swarm.Syncable.prototype.newEventSpec)
- description and source-code
```javascript
newEventSpec = function (op) {
    return this.spec().add(this._host.time(), '!').add(op, '.');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.off"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>off ()](#apidoc.element.swarm.Syncable.prototype.off)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
...

/**
 * Unsubscribe from collections entries' events
 * @param {function(*)} callback
 * @this Set|Vector
 */
offObjectEvent: function (callback) {
    this._proxy.off(callback);
},

/**
 * Waits for collection to receive state from cache or uplink and then invokes passed callback
 *
 * @param {function()} callback
 * @this Set|Vector
...
```

#### <a name="apidoc.element.swarm.Syncable.prototype.on"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>on ()](#apidoc.element.swarm.Syncable.prototype.on)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.Syncable.prototype.once"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>once (filter, cb)](#apidoc.element.swarm.Syncable.prototype.once)
- description and source-code
```javascript
once = function (filter, cb) {
    this.on(filter, function onceWrap(spec, val, src) {
        // "this" is the object (Syncable)
        if (cb.constructor === Function) {
            cb.call(this, spec, val, src);
        } else {
            cb.deliver(spec, val, src);
        }
        this.off(filter, onceWrap);
    });
}
```
- example usage
```shell
...
    });
    if (!notInitedYet.length) {
        // all entries are inited
        callback();
    } else {
        // wait for some entry not ready yet
        var randomIdx = (Math.random() * (notInitedYet.length - 1)) | 0;
        notInitedYet[randomIdx].once('init', checker);
    }
}
if (this._version) {
    checker();
} else {
    this.once('init', checker);
}
...
```

#### <a name="apidoc.element.swarm.Syncable.prototype.pojo"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>pojo (addVersionInfo)](#apidoc.element.swarm.Syncable.prototype.pojo)
- description and source-code
```javascript
pojo = function (addVersionInfo) {
    var pojo = {},
        defs = this.constructor.defaults;
    for (var key in this) {
        if (this.hasOwnProperty(key)) {
            if (Syncable.reFieldName.test(key) && this[key] !== undefined) {
                var def = defs[key],
                    val = this[key];
                pojo[key] = def && def.type ?
                (val.toJSON && val.toJSON()) || val.toString() :
                        (val && val._id ? val._id : val); // TODO prettify
            }
        }
    }
    if (addVersionInfo) {
        pojo._id = this._id; // not necassary
        pojo._version = this._version;
        this._vector && (pojo._vector = this._vector);
        this._oplog && (pojo._oplog = this._oplog); //TODO copy
    }
    return pojo;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.reoff"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>reoff ()](#apidoc.element.swarm.Syncable.prototype.reoff)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.reon"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>reon ()](#apidoc.element.swarm.Syncable.prototype.reon)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.reset"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>reset ()](#apidoc.element.swarm.Syncable.prototype.reset)
- description and source-code
```javascript
reset = function () {
    var defs = this.constructor.defaults;
    for (var name in defs) {
        var def = defs[name];
        if (def.type) {
            this[name] = def.value ? new def.type(def.value) : new def.type();
        } else {
            this[name] = def.value;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.spec"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>spec ()](#apidoc.element.swarm.Syncable.prototype.spec)
- description and source-code
```javascript
spec = function () { return new Spec('/' + this._type + '#' + this._id); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.stateSpec"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>stateSpec ()](#apidoc.element.swarm.Syncable.prototype.stateSpec)
- description and source-code
```javascript
stateSpec = function () {
    return this.spec() + (this._version || ''); //?
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.trigger"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>trigger (event, params)](#apidoc.element.swarm.Syncable.prototype.trigger)
- description and source-code
```javascript
trigger = function (event, params) {
    var spec = this.newEventSpec(event);
    this.deliver(spec, params);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.unimplemented"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>unimplemented (spec, val, repl)](#apidoc.element.swarm.Syncable.prototype.unimplemented)
- description and source-code
```javascript
unimplemented = function (spec, val, repl) {
    console.warn("method not implemented:", spec);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.validate"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>validate (spec, val, src)](#apidoc.element.swarm.Syncable.prototype.validate)
- description and source-code
```javascript
validate = function (spec, val, src) {
    if (spec.pattern() !== '/#!.') {
        return 'incomplete event spec';
    }
    if (this.clock && spec.type()!=='Host' && !this.clock.checkTimestamp(spec.version())) {
        return 'invalid timestamp '+spec;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype.version"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype.</span>version ()](#apidoc.element.swarm.Syncable.prototype.version)
- description and source-code
```javascript
version = function () {
    // distillLog() may drop some operations; still, those need to be counted
    // in the version vector; so, their Lamport ids must be saved in this._vector
    var map = new Spec.Map(this._version + (this._vector || ''));
    if (this._oplog) {
        for (var op in this._oplog) {
            map.add(op);
        }
    }
    return map; // TODO return the object, let the consumer trim it to taste
}
```
- example usage
```shell
...
    }
    this.weave = w1.join('');
    this.ids = w4;
    this.rebuild();
},
remove: function (spec, rm, src) {
    var w1 = [], w4 = [];
    var v = spec.version();
    for (var i = 0; i < this.weave.length; i++) {
        w1.push(this.weave.charAt(i));
        w4.push(this.ids[i]);
        if (this.ids[i] in rm) {
            w1.push('\u0008');
            w4.push(v);
        }
...
```



# <a name="apidoc.module.swarm.Syncable.prototype._neutrals"></a>[module swarm.Syncable.prototype._neutrals](#apidoc.module.swarm.Syncable.prototype._neutrals)

#### <a name="apidoc.element.swarm.Syncable.prototype._neutrals.error"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype._neutrals.</span>error (spec, val, repl)](#apidoc.element.swarm.Syncable.prototype._neutrals.error)
- description and source-code
```javascript
error = function (spec, val, repl) {
    console.error('something failed:', spec, val, '@', (repl && repl._id));
}
```
- example usage
```shell
...
        this.buf = buf; //will wait for "open"
    }
    ws.on('close', function () { ln.close && ln.close(); });
    ws.on('data', function (msg) {
        try {
            ln.data && ln.data(msg);
        } catch (ex) {
            console.error('message processing fails', ex);
            ln.error && ln.error(ex.message);
        }
    });
}

module.exports = SockJSStream;
...
```

#### <a name="apidoc.element.swarm.Syncable.prototype._neutrals.off"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype._neutrals.</span>off (spec, val, repl)](#apidoc.element.swarm.Syncable.prototype._neutrals.off)
- description and source-code
```javascript
off = function (spec, val, repl) {
    var idx = this.getListenerIndex(repl); //TODO ??? uplinks_only?
    if (idx > -1) {
        this._lstn.splice(idx, 1);
    }
}
```
- example usage
```shell
...

/**
 * Unsubscribe from collections entries' events
 * @param {function(*)} callback
 * @this Set|Vector
 */
offObjectEvent: function (callback) {
    this._proxy.off(callback);
},

/**
 * Waits for collection to receive state from cache or uplink and then invokes passed callback
 *
 * @param {function()} callback
 * @this Set|Vector
...
```

#### <a name="apidoc.element.swarm.Syncable.prototype._neutrals.on"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype._neutrals.</span>on (spec, filter, repl)](#apidoc.element.swarm.Syncable.prototype._neutrals.on)
- description and source-code
```javascript
on = function (spec, filter, repl) {   // WELL  on() is not an op, right?
    // if no listener is supplied then the object is only
    // guaranteed to exist till the next Host.gc() run
    if (!repl) { return; }

    var self = this;
    // stateless objects fire no events; essentially, on() is deferred
    if (!this._version && filter) { // TODO solidify
        this._lstn.push({
            _op: 'reon',
            _src: repl,
            deliver: function () {
                var i = self._lstn.indexOf(this);
                self._lstn.splice(i, 1);
                self.deliver(spec, filter, repl);
            }
        });
        return; // defer this call till uplinks are ready
    }
    // make all listeners uniform objects
    if (repl.constructor === Function) {
        repl = {
            sink: repl,
            that: this,
            deliver: function () { // .deliver is invoked on an event
                this.sink.apply(this.that, arguments);
            }
        };
    }

    if (filter) {
        filter = new Spec(filter, '.');
        var baseVersion = filter.filter('!'),
            filter_by_op = filter.get('.');

        if (filter_by_op === 'init') {
            var diff_if_needed = baseVersion ? this.diff(baseVersion) : '';
            repl.deliver(spec.set('.init'), diff_if_needed, this); //??
            // FIXME use once()
            return;
        }
        if (filter_by_op) {
            repl = {
                sink: repl,
                _op: filter_by_op,
                deliver: function deliverWithFilter(spec, val, src) {
                    if (spec.op() === filter_by_op) {
                        this.sink.deliver(spec, val, src);
                    }
                }
            };
        }

        if (!baseVersion.isEmpty()) {
            var diff = this.diff(baseVersion);
            diff && repl.deliver(spec.set('.init'), diff, this); // 2downlink
            repl.deliver(spec.set('.reon'), this.version().toString(), this);
        }
    }

    this._lstn.push(repl);
    // TODO repeated subscriptions: send a diff, otherwise ignore
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.Syncable.prototype._neutrals.reoff"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype._neutrals.</span>reoff (spec, val, repl)](#apidoc.element.swarm.Syncable.prototype._neutrals.reoff)
- description and source-code
```javascript
reoff = function (spec, val, repl) {
    var idx = this.getListenerIndex(repl); //TODO ??? uplinks_only?
    if (idx > -1) {
        this._lstn.splice(idx, 1);
    }
    if (this._id) {
        this.checkUplink();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.prototype._neutrals.reon"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype._neutrals.</span>reon (spec, filter, repl)](#apidoc.element.swarm.Syncable.prototype._neutrals.reon)
- description and source-code
```javascript
reon = function (spec, filter, repl) {
    if (filter) {  // a diff is requested
        var base = Spec.as(filter).tok('!');
        var diff = this.diff(base);
        if (diff) {
            repl.deliver(spec.set('.init'), diff, this);
        }
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Syncable.prototype._ops"></a>[module swarm.Syncable.prototype._ops](#apidoc.module.swarm.Syncable.prototype._ops)

#### <a name="apidoc.element.swarm.Syncable.prototype._ops.init"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.prototype._ops.</span>init (spec, state, src)](#apidoc.element.swarm.Syncable.prototype._ops.init)
- description and source-code
```javascript
init = function (spec, state, src) {

    var tail = {}, // ops to be applied on top of the received state
        typeid = spec.filter('/#'),
        lstn = this._lstn,
        a_spec;
    this._lstn = []; // prevent events from being fired

    if (state._version/* && state._version !== '!0'*/) {
        // local changes may need to be merged into the received state
        if (this._oplog) {
            for (a_spec in this._oplog) {
                tail[a_spec] = this._oplog[a_spec];
            }
            this._oplog = {};
        }
        this._vector && (this._vector = undefined);
        // zero everything
        for (var key in this) {
            if (this.hasOwnProperty(key) && key.charAt(0) !== '_') {
                this[key] = undefined;
            }
        }
        // set default values
        this.reset();

        this.apply(state);
        this._version = state._version;

        state._oplog && (this._oplog = state._oplog); // FIXME copy
        state._vector && (this._vector = state._vector);
    }
    // add the received tail to the local one
    if (state._tail) {
        for (a_spec in state._tail) {
            tail[a_spec] = state._tail[a_spec];
        }
    }
    // appply the combined tail to the new state
    var specs = [];
    for (a_spec in tail) {
        specs.push(a_spec);
    }
    specs.sort().reverse();
    // there will be some replays, but those will be ignored
    while (a_spec = specs.pop()) {
        this.deliver(typeid.add(a_spec), tail[a_spec], this);
    }

    this._lstn = lstn;

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Syncable.types"></a>[module swarm.Syncable.types](#apidoc.module.swarm.Syncable.types)

#### <a name="apidoc.element.swarm.Syncable.types.Host"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.</span>Host (id, ms, storage)](#apidoc.element.swarm.Syncable.types.Host)
- description and source-code
```javascript
function Host(id, ms, storage) {
    this.objects = {};
    this.sources = {};
    this.storage = storage;
    this._host = this; // :)
    this._lstn = [','];
    this._id = id;
    this._server = /^swarm~.*/.test(id);
    var clock_fn = env.clockType || SecondPreciseClock;
    this.clock = new clock_fn(this._id, ms||0);

    if (this.storage) {
        this.sources[this._id] = this.storage;
        this.storage._host = this;
    }
    delete this.objects[this.spec()];

    if (!env.multihost) {
        if (env.localhost) {
            throw new Error('use multihost mode');
        }
        env.localhost = this;
    }
}
```
- example usage
```shell
...
module.exports = Mouse; // CommonJS
'''

### Using the model on the client (app.js)

'''js
// 1. create local Host
var swarmHost = new Swarm.Host('unique_client_id');

// 2. connect to your server
swarmHost.connect('ws://localhost:8000/');

// 3.a. create an object
var someMouse = new Mouse();
// OR swarmHost.get('/Mouse');
...
```

#### <a name="apidoc.element.swarm.Syncable.types.Model"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.</span>Model (idOrState)](#apidoc.element.swarm.Syncable.types.Model)
- description and source-code
```javascript
function Model(idOrState) {
    var ret = Model._super.apply(this, arguments);
    /// TODO: combine with state push, make clean
    if (ret === this && idOrState && idOrState.constructor !== String && !Spec.is(idOrState)) {
        this.deliver(this.spec().add(this._id, '!').add('.set'), idOrState);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.types.Set"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.</span>Set ()](#apidoc.element.swarm.Syncable.types.Set)
- description and source-code
```javascript
function SomeSyncable() {
    return parent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.types.Syncable"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.</span>Syncable ()](#apidoc.element.swarm.Syncable.types.Syncable)
- description and source-code
```javascript
function Syncable() {
    // listeners represented as objects that have deliver() method
    this._lstn = [',']; // we unshift() uplink listeners and push() downlinks
    // ...so _lstn is like [server1, server2, storage, ',', view, listener]
    // The most correct way to specify a version is the version vector,
    // but that one may consume more space than the data itself in some cases.
    // Hence, _version is not a fully specified version vector (see version()
    // instead). _version is essentially is the greatest operation timestamp
    // (Lamport-like, i.e. "time+source"), sometimes amended with additional
    // timestamps. Its main features:
    // (1) changes once the object's state changes
    // (2) does it monotonically (in the alphanum order sense)
    this._version = '';
    // make sense of arguments
    var args = Array.prototype.slice.call(arguments);
    this._host = (args.length && args[args.length - 1]._type === 'Host') ?
            args.pop() : env.localhost;
    if (Spec.is(args[0])) {
        this._id = new Spec(args.shift()).id() || this._host.time();
    } else if (typeof(args[0]) === 'string') {
        this._id = args.shift(); // TODO format
    } else {
        this._id = this._host.time();
        this._version = '!0'; // may apply state in the constructor, see Model
    }
    //var state = args.length ? args.pop() : (fresh?{}:undefined);
    // register with the host
    var doubl = this._host.register(this);
    if (doubl !== this) { return doubl; }
    // locally created objects get state immediately
    // (while external-id objects need to query uplinks)
<span class="apidocCodeCommentSpan">    /*if (fresh && state) {
     state._version = '!'+this._id;
     var pspec = this.spec().add(state._version).add('.init');
     this.deliver(pspec,state,this._host);
     }*/
</span>    this.reset();
    // find uplinks, subscribe
    this.checkUplink();
    // TODO inplement state push
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.types.Text"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.</span>Text ()](#apidoc.element.swarm.Syncable.types.Text)
- description and source-code
```javascript
function SomeSyncable() {
    return parent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.types.Vector"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.</span>Vector ()](#apidoc.element.swarm.Syncable.types.Vector)
- description and source-code
```javascript
function SomeSyncable() {
    return parent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Syncable.types.Text.prototype"></a>[module swarm.Syncable.types.Text.prototype](#apidoc.module.swarm.Syncable.types.Text.prototype)

#### <a name="apidoc.element.swarm.Syncable.types.Text.prototype.callReactions"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>callReactions (spec, value, src)](#apidoc.element.swarm.Syncable.types.Text.prototype.callReactions)
- description and source-code
```javascript
callReactions = function (spec, value, src) {
    var superReactions = syncProto._super.callReactions;
    if ('function' === typeof superReactions) {
        superReactions.call(this, spec, value, src);
    }
    var r = syncProto._reactions[spec.op()];
    if (r) {
        r.constructor !== Array && (r = [r]);
        for (var i = 0; i < r.length; i++) {
            r[i] && r[i].call(this, spec, value, src);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.types.Text.prototype.constructor"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>constructor ()](#apidoc.element.swarm.Syncable.types.Text.prototype.constructor)
- description and source-code
```javascript
function SomeSyncable() {
    return parent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Syncable.types.Text.prototype.insert"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>insert ()](#apidoc.element.swarm.Syncable.types.Text.prototype.insert)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
...
            }
            break;
        case '=':
            skip(val.length);
        }
    }
    rm && this.remove(rm);
    ins && this.insert(ins);
}
});

Text.diff = function diff(was, is) {
var ret = [];
// prefix suffix the rest is change
var pre = 0;
...
```

#### <a name="apidoc.element.swarm.Syncable.types.Text.prototype.rebuild"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>rebuild ()](#apidoc.element.swarm.Syncable.types.Text.prototype.rebuild)
- description and source-code
```javascript
rebuild = function () {
<span class="apidocCodeCommentSpan">    /*var re = /([^\u0008][\u0008]+)|([^\u0008])/g, m=[];
     var text = [], tids = [], pos = 0;
     while (m=re.exec(this.weave)) {
     if (m[2]) {
     text.push(m[2]);
     tids.push(this.ids[pos]);
     }
     pos += m[0].length;
     }

     this.tids = tids;*/
</span>    this.text = this.weave.replace(/[^\u0008][\u0008]+/mg, '').substr(1);
}
```
- example usage
```shell
...
        }
    }
    if (genTs) {
        this._host.clock.checkTimestamp(genTs);
    }
    this.weave = w1.join('');
    this.ids = w4;
    this.rebuild();
},
remove: function (spec, rm, src) {
    var w1 = [], w4 = [];
    var v = spec.version();
    for (var i = 0; i < this.weave.length; i++) {
        w1.push(this.weave.charAt(i));
        w4.push(this.ids[i]);
...
```

#### <a name="apidoc.element.swarm.Syncable.types.Text.prototype.remove"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>remove ()](#apidoc.element.swarm.Syncable.types.Text.prototype.remove)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
...
                skip();
            }
            break;
        case '=':
            skip(val.length);
        }
    }
    rm && this.remove(rm);
    ins && this.insert(ins);
}
});

Text.diff = function diff(was, is) {
var ret = [];
// prefix suffix the rest is change
...
```

#### <a name="apidoc.element.swarm.Syncable.types.Text.prototype.set"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>set (newText)](#apidoc.element.swarm.Syncable.types.Text.prototype.set)
- description and source-code
```javascript
set = function (newText) {
    var patch = Text.diff(this.text, newText);
    var rm = null, ins = null, weave = this.weave;
    var re_atom = /[^\u0008]([^\u0008][\u0008]+)*/mg;
    var atom;

    function skip(n) {
        for (n = n || 1; n > 0; n--) {
            atom = re_atom.exec(weave);
        }
    }

    skip(1); // \n #00000+swarm

    for (var i = 0; i < patch.length; i++) {
        var op = patch[i][0], val = patch[i][1];
        switch (op) {
        case '+':
            ins || (ins = {});
            ins[this.ids[atom.index]] = val;
            break;
        case '-':
            rm || (rm = {});
            for (var r = 0; r < val.length; r++) {
                rm[this.ids[atom.index + atom[0].length]] = true;
                skip();
            }
            break;
        case '=':
            skip(val.length);
        }
    }
    rm && this.remove(rm);
    ins && this.insert(ins);
}
```
- example usage
```shell
...

// 3.a. create an object
var someMouse = new Mouse();
// OR swarmHost.get('/Mouse');
// OR new Mouse({x:1, y:2});

// 4.a. a locally created object may be touched immediately
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
...
```

#### <a name="apidoc.element.swarm.Syncable.types.Text.prototype.state"></a>[function <span class="apidocSignatureSpan">swarm.Syncable.types.Text.prototype.</span>state ()](#apidoc.element.swarm.Syncable.types.Text.prototype.state)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Text"></a>[module swarm.Text](#apidoc.module.swarm.Text)

#### <a name="apidoc.element.swarm.Text.Text"></a>[function <span class="apidocSignatureSpan">swarm.</span>Text ()](#apidoc.element.swarm.Text.Text)
- description and source-code
```javascript
function SomeSyncable() {
    return parent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Text._super"></a>[function <span class="apidocSignatureSpan">swarm.Text.</span>_super ()](#apidoc.element.swarm.Text._super)
- description and source-code
```javascript
function Syncable() {
    // listeners represented as objects that have deliver() method
    this._lstn = [',']; // we unshift() uplink listeners and push() downlinks
    // ...so _lstn is like [server1, server2, storage, ',', view, listener]
    // The most correct way to specify a version is the version vector,
    // but that one may consume more space than the data itself in some cases.
    // Hence, _version is not a fully specified version vector (see version()
    // instead). _version is essentially is the greatest operation timestamp
    // (Lamport-like, i.e. "time+source"), sometimes amended with additional
    // timestamps. Its main features:
    // (1) changes once the object's state changes
    // (2) does it monotonically (in the alphanum order sense)
    this._version = '';
    // make sense of arguments
    var args = Array.prototype.slice.call(arguments);
    this._host = (args.length && args[args.length - 1]._type === 'Host') ?
            args.pop() : env.localhost;
    if (Spec.is(args[0])) {
        this._id = new Spec(args.shift()).id() || this._host.time();
    } else if (typeof(args[0]) === 'string') {
        this._id = args.shift(); // TODO format
    } else {
        this._id = this._host.time();
        this._version = '!0'; // may apply state in the constructor, see Model
    }
    //var state = args.length ? args.pop() : (fresh?{}:undefined);
    // register with the host
    var doubl = this._host.register(this);
    if (doubl !== this) { return doubl; }
    // locally created objects get state immediately
    // (while external-id objects need to query uplinks)
<span class="apidocCodeCommentSpan">    /*if (fresh && state) {
     state._version = '!'+this._id;
     var pspec = this.spec().add(state._version).add('.init');
     this.deliver(pspec,state,this._host);
     }*/
</span>    this.reset();
    // find uplinks, subscribe
    this.checkUplink();
    // TODO inplement state push
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Text.addReaction"></a>[function <span class="apidocSignatureSpan">swarm.Text.</span>addReaction (op, fn)](#apidoc.element.swarm.Text.addReaction)
- description and source-code
```javascript
addReaction = function (op, fn) {
    var reactions = this.prototype._reactions;
    var list = reactions[op];
    list || (list = reactions[op] = []);
    list.push(fn);
    return {op: op, fn: fn};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Text.diff"></a>[function <span class="apidocSignatureSpan">swarm.Text.</span>diff (was, is)](#apidoc.element.swarm.Text.diff)
- description and source-code
```javascript
function diff(was, is) {
    var ret = [];
    // prefix suffix the rest is change
    var pre = 0;
    while (pre < was.length && pre < is.length && was.charAt(pre) === is.charAt(pre)) {
        pre++;
    }
    var post = 0;
    while (post < was.length - pre && post < is.length - pre &&
    was.charAt(was.length - post - 1) === is.charAt(is.length - post - 1)) {
        post++;
    }
    if (pre) {
        ret.push(['=', was.substr(0, pre)]);
    }
    var ins = is.length - pre - post;
    if (ins) {
        ret.push(['+', is.substr(pre, ins)]);
    }
    var rm = was.length - pre - post;
    if (rm) {
        ret.push(['-', was.substr(pre, rm)]);
    }
    if (post) {
        ret.push(['=', was.substr(pre + rm)]);
    }
    return ret;

}
```
- example usage
```shell
...
 pos += m[0].length;
 }

 this.tids = tids;*/
this.text = this.weave.replace(/[^\u0008][\u0008]+/mg, '').substr(1);
    },
    set: function (newText) {
var patch = Text.diff(this.text, newText);
var rm = null, ins = null, weave = this.weave;
var re_atom = /[^\u0008]([^\u0008][\u0008]+)*/mg;
var atom;

function skip(n) {
    for (n = n || 1; n > 0; n--) {
        atom = re_atom.exec(weave);
...
```

#### <a name="apidoc.element.swarm.Text.extend"></a>[function <span class="apidocSignatureSpan">swarm.Text.</span>extend (fn, own)](#apidoc.element.swarm.Text.extend)
- description and source-code
```javascript
extend = function (fn, own) {
    var parent = this, fnid;
    if (fn.constructor !== Function) {
        var id = fn.toString();
        fn = function SomeSyncable() {
            return parent.apply(this, arguments);
        };
        fnid = id; // if only it worked
    } else { // please call Syncable.constructor.apply(this,args) in your constructor
        fnid = fnname(fn);
    }

    // inheritance trick from backbone.js
    var SyncProto = function () {
        this.constructor = fn;
        this._neutrals = {};
        this._ops = {};
        this._reactions = {};

        var event,
            name;
        if (parent._pt) {
            //copy _neutrals & _ops from parent
            for (event in parent._pt._neutrals) {
                this._neutrals[event] = parent._pt._neutrals[event];
            }
            for (event in parent._pt._ops) {
                this._ops[event] = parent._pt._ops[event];
            }
        }

        // "Methods" are serialized, logged and delivered to replicas
        for (name in own.ops || {}) {
            if (Syncable.reMethodName.test(name)) {
                this._ops[name] = own.ops[name];
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid op name:',name);
            }
        }

        // "Neutrals" don't change the state
        for (name in own.neutrals || {}) {
            if (Syncable.reMethodName.test(name)) {
                this._neutrals[name] = own.neutrals[name];
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid neutral op name:',name);
            }
        }

        // "Remotes" are serialized and sent upstream (like RPC calls)
        for (name in own.remotes || {}) {
            if (Syncable.reMethodName.test(name)) {
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid rpc name:',name);
            }
        }

        // add mixins
        (own.mixins || []).forEach(function (mixin) {
            for (var name in mixin) {
                this[name] = mixin[name];
            }
        }, this);

        // add other members
        for (name in own) {
            if (Syncable.reMethodName.test(name)) {
                var memberType = own[name].constructor;
                if (memberType === Function) { // non-op method
                    // these must change state ONLY by invoking ops
                    this[name] = own[name];
                } else if (memberType===String || memberType===Number) {
                    this[name] = own[name]; // some static constant, OK
                } else if (name in Syncable.memberClasses) {
                    // see above
                    continue;
                } else {
                    console.warn('invalid member:',name,memberType);
                }
            } else {
                console.warn('invalid member name:',name);
            }
        }

        // add reactions
        for (name in own.reactions || {}) {
            var reaction = own.reactions[name];
            if (!reaction) { continue; }

            switch (typeof reaction) {
            case 'function':
                // handler-function
                this._reactions[name] = [reaction];
                break;
            case 'string':
                // handler-method name
                this._reactions[name] = [this[name]];
                break;
            default:
                if (reaction.constructor === Array) {
                    // array of handlers
                    this._reactions[name] = reaction.map(function (item) {
                        switch (typeof item) {
                        case 'function':
                            return item;
                        case 'string':
                            return this[item];
                        default:
                            throw new Error('unexpected reaction type');
                        }
                    }, this);
                } else {
                    throw new Error('unex ...
```
- example usage
```shell
...
these demos are normally online at http://ppyr.us and http://ppyr.us:8001/demo3/index.html respectively.

### Creating your first simple synchronized type

'''js
var Swarm = require('swarm');

var Mouse = Swarm.Model.extend('Mouse', {
    defaults: {
        name: 'Mickey',
        x: 0,
        y: 0
    }
});
...
```

#### <a name="apidoc.element.swarm.Text.removeReaction"></a>[function <span class="apidocSignatureSpan">swarm.Text.</span>removeReaction (handle)](#apidoc.element.swarm.Text.removeReaction)
- description and source-code
```javascript
removeReaction = function (handle) {
    var op = handle.op,
        fn = handle.fn,
        list = this.prototype._reactions[op],
        i = list.indexOf(fn);
    if (i === -1) {
        throw new Error('reaction unknown');
    }
    list[i] = undefined; // such a peculiar pattern not to mess up out-of-callback removal
    while (list.length && !list[list.length - 1]) {
        list.pop();
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Vector"></a>[module swarm.Vector](#apidoc.module.swarm.Vector)

#### <a name="apidoc.element.swarm.Vector.Vector"></a>[function <span class="apidocSignatureSpan">swarm.</span>Vector ()](#apidoc.element.swarm.Vector.Vector)
- description and source-code
```javascript
function SomeSyncable() {
    return parent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector._super"></a>[function <span class="apidocSignatureSpan">swarm.Vector.</span>_super ()](#apidoc.element.swarm.Vector._super)
- description and source-code
```javascript
function Syncable() {
    // listeners represented as objects that have deliver() method
    this._lstn = [',']; // we unshift() uplink listeners and push() downlinks
    // ...so _lstn is like [server1, server2, storage, ',', view, listener]
    // The most correct way to specify a version is the version vector,
    // but that one may consume more space than the data itself in some cases.
    // Hence, _version is not a fully specified version vector (see version()
    // instead). _version is essentially is the greatest operation timestamp
    // (Lamport-like, i.e. "time+source"), sometimes amended with additional
    // timestamps. Its main features:
    // (1) changes once the object's state changes
    // (2) does it monotonically (in the alphanum order sense)
    this._version = '';
    // make sense of arguments
    var args = Array.prototype.slice.call(arguments);
    this._host = (args.length && args[args.length - 1]._type === 'Host') ?
            args.pop() : env.localhost;
    if (Spec.is(args[0])) {
        this._id = new Spec(args.shift()).id() || this._host.time();
    } else if (typeof(args[0]) === 'string') {
        this._id = args.shift(); // TODO format
    } else {
        this._id = this._host.time();
        this._version = '!0'; // may apply state in the constructor, see Model
    }
    //var state = args.length ? args.pop() : (fresh?{}:undefined);
    // register with the host
    var doubl = this._host.register(this);
    if (doubl !== this) { return doubl; }
    // locally created objects get state immediately
    // (while external-id objects need to query uplinks)
<span class="apidocCodeCommentSpan">    /*if (fresh && state) {
     state._version = '!'+this._id;
     var pspec = this.spec().add(state._version).add('.init');
     this.deliver(pspec,state,this._host);
     }*/
</span>    this.reset();
    // find uplinks, subscribe
    this.checkUplink();
    // TODO inplement state push
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.addReaction"></a>[function <span class="apidocSignatureSpan">swarm.Vector.</span>addReaction (op, fn)](#apidoc.element.swarm.Vector.addReaction)
- description and source-code
```javascript
addReaction = function (op, fn) {
    var reactions = this.prototype._reactions;
    var list = reactions[op];
    list || (list = reactions[op] = []);
    list.push(fn);
    return {op: op, fn: fn};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.extend"></a>[function <span class="apidocSignatureSpan">swarm.Vector.</span>extend (fn, own)](#apidoc.element.swarm.Vector.extend)
- description and source-code
```javascript
extend = function (fn, own) {
    var parent = this, fnid;
    if (fn.constructor !== Function) {
        var id = fn.toString();
        fn = function SomeSyncable() {
            return parent.apply(this, arguments);
        };
        fnid = id; // if only it worked
    } else { // please call Syncable.constructor.apply(this,args) in your constructor
        fnid = fnname(fn);
    }

    // inheritance trick from backbone.js
    var SyncProto = function () {
        this.constructor = fn;
        this._neutrals = {};
        this._ops = {};
        this._reactions = {};

        var event,
            name;
        if (parent._pt) {
            //copy _neutrals & _ops from parent
            for (event in parent._pt._neutrals) {
                this._neutrals[event] = parent._pt._neutrals[event];
            }
            for (event in parent._pt._ops) {
                this._ops[event] = parent._pt._ops[event];
            }
        }

        // "Methods" are serialized, logged and delivered to replicas
        for (name in own.ops || {}) {
            if (Syncable.reMethodName.test(name)) {
                this._ops[name] = own.ops[name];
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid op name:',name);
            }
        }

        // "Neutrals" don't change the state
        for (name in own.neutrals || {}) {
            if (Syncable.reMethodName.test(name)) {
                this._neutrals[name] = own.neutrals[name];
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid neutral op name:',name);
            }
        }

        // "Remotes" are serialized and sent upstream (like RPC calls)
        for (name in own.remotes || {}) {
            if (Syncable.reMethodName.test(name)) {
                this[name] = wrapCall(name);
            } else {
                console.warn('invalid rpc name:',name);
            }
        }

        // add mixins
        (own.mixins || []).forEach(function (mixin) {
            for (var name in mixin) {
                this[name] = mixin[name];
            }
        }, this);

        // add other members
        for (name in own) {
            if (Syncable.reMethodName.test(name)) {
                var memberType = own[name].constructor;
                if (memberType === Function) { // non-op method
                    // these must change state ONLY by invoking ops
                    this[name] = own[name];
                } else if (memberType===String || memberType===Number) {
                    this[name] = own[name]; // some static constant, OK
                } else if (name in Syncable.memberClasses) {
                    // see above
                    continue;
                } else {
                    console.warn('invalid member:',name,memberType);
                }
            } else {
                console.warn('invalid member name:',name);
            }
        }

        // add reactions
        for (name in own.reactions || {}) {
            var reaction = own.reactions[name];
            if (!reaction) { continue; }

            switch (typeof reaction) {
            case 'function':
                // handler-function
                this._reactions[name] = [reaction];
                break;
            case 'string':
                // handler-method name
                this._reactions[name] = [this[name]];
                break;
            default:
                if (reaction.constructor === Array) {
                    // array of handlers
                    this._reactions[name] = reaction.map(function (item) {
                        switch (typeof item) {
                        case 'function':
                            return item;
                        case 'string':
                            return this[item];
                        default:
                            throw new Error('unexpected reaction type');
                        }
                    }, this);
                } else {
                    throw new Error('unex ...
```
- example usage
```shell
...
these demos are normally online at http://ppyr.us and http://ppyr.us:8001/demo3/index.html respectively.

### Creating your first simple synchronized type

'''js
var Swarm = require('swarm');

var Mouse = Swarm.Model.extend('Mouse', {
    defaults: {
        name: 'Mickey',
        x: 0,
        y: 0
    }
});
...
```

#### <a name="apidoc.element.swarm.Vector.removeReaction"></a>[function <span class="apidocSignatureSpan">swarm.Vector.</span>removeReaction (handle)](#apidoc.element.swarm.Vector.removeReaction)
- description and source-code
```javascript
removeReaction = function (handle) {
    var op = handle.op,
        fn = handle.fn,
        list = this.prototype._reactions[op],
        i = list.indexOf(fn);
    if (i === -1) {
        throw new Error('reaction unknown');
    }
    list[i] = undefined; // such a peculiar pattern not to mess up out-of-callback removal
    while (list.length && !list[list.length - 1]) {
        list.pop();
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Vector.prototype"></a>[module swarm.Vector.prototype](#apidoc.module.swarm.Vector.prototype)

#### <a name="apidoc.element.swarm.Vector.prototype.addObject"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>addObject (obj)](#apidoc.element.swarm.Vector.prototype.addObject)
- description and source-code
```javascript
addObject = function (obj) {
    this.append(obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.append"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>append (spec)](#apidoc.element.swarm.Vector.prototype.append)
- description and source-code
```javascript
function append(spec) {
    this.insert(spec,this._order.length()-1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.callReactions"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>callReactions (spec, value, src)](#apidoc.element.swarm.Vector.prototype.callReactions)
- description and source-code
```javascript
callReactions = function (spec, value, src) {
    var superReactions = syncProto._super.callReactions;
    if ('function' === typeof superReactions) {
        superReactions.call(this, spec, value, src);
    }
    var r = syncProto._reactions[spec.op()];
    if (r) {
        r.constructor !== Array && (r = [r]);
        for (var i = 0; i < r.length; i++) {
            r[i] && r[i].call(this, spec, value, src);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.constructor"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>constructor ()](#apidoc.element.swarm.Vector.prototype.constructor)
- description and source-code
```javascript
function SomeSyncable() {
    return parent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.distillLog"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>distillLog ()](#apidoc.element.swarm.Vector.prototype.distillLog)
- description and source-code
```javascript
distillLog = function () {
    // TODO HORIZON
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.every"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>every (cb, thisArg)](#apidoc.element.swarm.Vector.prototype.every)
- description and source-code
```javascript
every = function (cb, thisArg) {
    return this._objects.every(cb, thisArg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.filter"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>filter (cb, thisArg)](#apidoc.element.swarm.Vector.prototype.filter)
- description and source-code
```javascript
filter = function (cb, thisArg) {
    return this._objects.filter(cb, thisArg);
}
```
- example usage
```shell
...
 *
 * @param {function()} callback
 * @this Set|Vector
 */
onObjectStateReady: function (callback) { // TODO timeout ?
    var self = this;
    function checker() {
        var notInitedYet = self.filter(function (entry) {
            return !entry._version;
        });
        if (!notInitedYet.length) {
            // all entries are inited
            callback();
        } else {
            // wait for some entry not ready yet
...
```

#### <a name="apidoc.element.swarm.Vector.prototype.findPositionFor"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>findPositionFor (id, parentId)](#apidoc.element.swarm.Vector.prototype.findPositionFor)
- description and source-code
```javascript
findPositionFor = function (id, parentId) { // FIXME protected methods && statics (entryType)
    if (!parentId) {
        parentId = this.getParentOf(id);
    }
    var next;
    if (parentId!=='!0') {
        next = this._order.find(parentId);
        if (next.end()) {
            next = this.findPositionFor(parentId);
        }
        next.next();
    } else {
        next = this._order.iterator();
    }
    // skip "younger" concurrent siblings
    while (!next.end()) {
        var nextId = next.token();
        if (nextId<id) {
            break;
        }
        var subtreeId = this.inSubtreeOf(nextId,parentId);
        if (!subtreeId || subtreeId<id) {
            break;
        }
        this.skipSubtree(next,subtreeId);
    }
    return next; // insert before
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.forEach"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>forEach (cb, thisArg)](#apidoc.element.swarm.Vector.prototype.forEach)
- description and source-code
```javascript
forEach = function (cb, thisArg) {
    this._objects.forEach(cb, thisArg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.getObject"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>getObject (spec)](#apidoc.element.swarm.Vector.prototype.getObject)
- description and source-code
```javascript
getObject = function (spec) {
    spec = new Spec(spec,'#');
    if (!spec.has('/')) {
        if (this.objectType) {
            spec = spec.add(this.objectType.prototype._type,'/').sort();
        } else {
            throw new Error("type not specified"); // TODO is it necessary at all?
        }
    }
    var obj = this._host.get(spec);
    return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.getParentOf"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>getParentOf (id)](#apidoc.element.swarm.Vector.prototype.getParentOf)
- description and source-code
```javascript
getParentOf = function (id) {
    var spec = this._oplog[id+'.in'];
    if (!spec) {
        throw new Error('operation unknown: '+id);
    }
    var parentId = Spec.as(spec).tok('!') || '!0';
    return parentId;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.in"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>in ()](#apidoc.element.swarm.Vector.prototype.in)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.inSubtreeOf"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>inSubtreeOf (nodeId, rootId)](#apidoc.element.swarm.Vector.prototype.inSubtreeOf)
- description and source-code
```javascript
inSubtreeOf = function (nodeId, rootId) {
    var id=nodeId, p=id;
    while (id>rootId) {
        p=id;
        id=this.getParentOf(id);
    }
    return id===rootId && p;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>indexOf (obj, startAt)](#apidoc.element.swarm.Vector.prototype.indexOf)
- description and source-code
```javascript
indexOf = function (obj, startAt) {
    if (!obj._id) {
        obj = this.getObject(obj);
    }
    return this._objects.indexOf(obj,startAt);
}
```
- example usage
```shell
...
ProxyListener.prototype.on = function (callback) {
    if (this.callbacks===null) { this.callbacks = []; }
    this.callbacks.push(callback);
};

ProxyListener.prototype.off = function (callback) {
    if (this.callbacks===null) { return; }
    var i = this.callbacks.indexOf(callback);
    if (i!==-1) {
        this.callbacks.splice(i,1);
    } else {
        console.warn('listener unknown', callback);
    }
};
...
```

#### <a name="apidoc.element.swarm.Vector.prototype.insert"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>insert (spec, pos)](#apidoc.element.swarm.Vector.prototype.insert)
- description and source-code
```javascript
insert = function (spec, pos) {
    // TODO bulk insert: make'em siblings
    if (pos===undefined) {
        pos = -1; // TODO ? this._order.length()
    }
    if (pos.constructor!==Number) {
        pos = this.normalizePos(pos);
    }
    if (spec && spec._id) {
        spec = spec.spec();
    } else /*if (spec.constructor===String)*/ {
        spec = new Spec(spec,'#');
    }
    // TODO new object
    var opid = pos===-1 ? '!0' : this._order.tokenAt(pos);
    // TODO hint pos
    return this.in(spec+opid);
}
```
- example usage
```shell
...
            }
            break;
        case '=':
            skip(val.length);
        }
    }
    rm && this.remove(rm);
    ins && this.insert(ins);
}
});

Text.diff = function diff(was, is) {
var ret = [];
// prefix suffix the rest is change
var pre = 0;
...
```

#### <a name="apidoc.element.swarm.Vector.prototype.insertAfter"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>insertAfter (obj, pos)](#apidoc.element.swarm.Vector.prototype.insertAfter)
- description and source-code
```javascript
insertAfter = function (obj, pos) {
    this.insert (obj,pos);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.insertBefore"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>insertBefore (spec, pos)](#apidoc.element.swarm.Vector.prototype.insertBefore)
- description and source-code
```javascript
insertBefore = function (spec, pos) {
    if (pos===undefined) {
        pos = this._order.length();
    }
    if (pos.constructor!==Number) {
        pos = this.normalizePos(pos);
    }
    this.insert(spec,pos-1);
}
```
- example usage
```shell
...
    /*
    var from=range.get('#'), till=range.get('#',from);
    // clean DOM range
    for(var pid=from; pid && pid!==till; pid=???)
        body.removeChild(pid);
    // install
    while ()
        body.insertBefore(newp,till); // TODO batch?
    // recover selection
    // */
};


//DOMEditor.prototype.getRTF = function (from, till, format, rtf) {
function dom2rtf (from, till, format, rtf) {
...
```

#### <a name="apidoc.element.swarm.Vector.prototype.insertSorted"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>insertSorted (obj, cmp)](#apidoc.element.swarm.Vector.prototype.insertSorted)
- description and source-code
```javascript
insertSorted = function (obj, cmp) {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.isDescendantOf"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>isDescendantOf (nodeId, rootId)](#apidoc.element.swarm.Vector.prototype.isDescendantOf)
- description and source-code
```javascript
isDescendantOf = function (nodeId, rootId) {
    var i=nodeId;
    while (i>rootId) {
        i=this.getParentOf(i);
    }
    return i===rootId;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.length"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>length ()](#apidoc.element.swarm.Vector.prototype.length)
- description and source-code
```javascript
length = function () {
    return this._objects.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.map"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>map (cb, thisArg)](#apidoc.element.swarm.Vector.prototype.map)
- description and source-code
```javascript
map = function (cb, thisArg) {
    return this._objects.map(cb, thisArg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.normalizePos"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>normalizePos (pos)](#apidoc.element.swarm.Vector.prototype.normalizePos)
- description and source-code
```javascript
normalizePos = function (pos) {
    if (pos && pos._id) {
        pos=pos._id;
    }
    var spec = new Spec(pos,'#');
    var type = spec.type();
    var id = spec.id();
    for(var i=0; i<this._objects.length; i++) {
        var obj = this._objects[i];
        if (obj && obj._id===id && (!type || obj._type===type)) {
            break;
        }
    }
    return i;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.objectAt"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>objectAt (i)](#apidoc.element.swarm.Vector.prototype.objectAt)
- description and source-code
```javascript
objectAt = function (i) {
    return this._objects[i];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.offObjectEvent"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>offObjectEvent (callback)](#apidoc.element.swarm.Vector.prototype.offObjectEvent)
- description and source-code
```javascript
offObjectEvent = function (callback) {
    this._proxy.off(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.onObjectEvent"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>onObjectEvent (callback)](#apidoc.element.swarm.Vector.prototype.onObjectEvent)
- description and source-code
```javascript
onObjectEvent = function (callback) {
    this._proxy.owner = this;
    this._proxy.on(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.onObjectStateReady"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>onObjectStateReady (callback)](#apidoc.element.swarm.Vector.prototype.onObjectStateReady)
- description and source-code
```javascript
onObjectStateReady = function (callback) { // TODO timeout ?
    var self = this;
    function checker() {
        var notInitedYet = self.filter(function (entry) {
            return !entry._version;
        });
        if (!notInitedYet.length) {
            // all entries are inited
            callback();
        } else {
            // wait for some entry not ready yet
            var randomIdx = (Math.random() * (notInitedYet.length - 1)) | 0;
            notInitedYet[randomIdx].once('init', checker);
        }
    }
    if (this._version) {
        checker();
    } else {
        this.once('init', checker);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.pojo"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>pojo ()](#apidoc.element.swarm.Vector.prototype.pojo)
- description and source-code
```javascript
pojo = function () {
    // invoke super.pojo()
    var result = Syncable._pt.pojo.apply(this, arguments);
    result.entries = Object.keys(this._objects);
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.remove"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>remove (pos)](#apidoc.element.swarm.Vector.prototype.remove)
- description and source-code
```javascript
function remove(pos) {
    if (pos.constructor!==Number) {
        pos = this.normalizePos(pos);
    }
    var hint = Spec.int2base(pos,0);
    var op = this._order.tokenAt(pos);
    this.rm(op+'.'+hint); // TODO generic spec quants
}
```
- example usage
```shell
...
                skip();
            }
            break;
        case '=':
            skip(val.length);
        }
    }
    rm && this.remove(rm);
    ins && this.insert(ins);
}
});

Text.diff = function diff(was, is) {
var ret = [];
// prefix suffix the rest is change
...
```

#### <a name="apidoc.element.swarm.Vector.prototype.removeObject"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>removeObject (pos)](#apidoc.element.swarm.Vector.prototype.removeObject)
- description and source-code
```javascript
removeObject = function (pos) {
    this.remove(pos);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.rm"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>rm ()](#apidoc.element.swarm.Vector.prototype.rm)
- description and source-code
```javascript
function wrapper() {
    // assign a Lamport timestamp
    var spec = this.newEventSpec(name);
    var args = Array.prototype.slice.apply(arguments), lstn;
    // find the callback if any
    Syncable.isOpSink(args[args.length - 1]) && (lstn = args.pop());
    // prettify the rest of the arguments
    if (!args.length) {  // FIXME isn't it confusing?
        args = ''; // used as 'empty'
    } else if (args.length === 1) {
        args = args[0]; // {key:val}
    }
    // TODO log 'initiated'
    return this.deliver(spec, args, lstn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.setOrder"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>setOrder (fn)](#apidoc.element.swarm.Vector.prototype.setOrder)
- description and source-code
```javascript
setOrder = function (fn) {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.skipSubtree"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>skipSubtree (iter, root)](#apidoc.element.swarm.Vector.prototype.skipSubtree)
- description and source-code
```javascript
skipSubtree = function (iter, root) {
    root = root || iter.token();
    do {
        iter.next();
    } while (!iter.end() && this.isDescendantOf(iter.token(),root));
    return iter;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype.validate"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype.</span>validate (spec, val, source)](#apidoc.element.swarm.Vector.prototype.validate)
- description and source-code
```javascript
validate = function (spec, val, source) {
    // ref op is known
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Vector.prototype._neutrals"></a>[module swarm.Vector.prototype._neutrals](#apidoc.module.swarm.Vector.prototype._neutrals)

#### <a name="apidoc.element.swarm.Vector.prototype._neutrals.error"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype._neutrals.</span>error (spec, val, repl)](#apidoc.element.swarm.Vector.prototype._neutrals.error)
- description and source-code
```javascript
error = function (spec, val, repl) {
    console.error('something failed:', spec, val, '@', (repl && repl._id));
}
```
- example usage
```shell
...
        this.buf = buf; //will wait for "open"
    }
    ws.on('close', function () { ln.close && ln.close(); });
    ws.on('data', function (msg) {
        try {
            ln.data && ln.data(msg);
        } catch (ex) {
            console.error('message processing fails', ex);
            ln.error && ln.error(ex.message);
        }
    });
}

module.exports = SockJSStream;
...
```

#### <a name="apidoc.element.swarm.Vector.prototype._neutrals.off"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype._neutrals.</span>off (spec, val, repl)](#apidoc.element.swarm.Vector.prototype._neutrals.off)
- description and source-code
```javascript
off = function (spec, val, repl) {
    var idx = this.getListenerIndex(repl); //TODO ??? uplinks_only?
    if (idx > -1) {
        this._lstn.splice(idx, 1);
    }
}
```
- example usage
```shell
...

/**
 * Unsubscribe from collections entries' events
 * @param {function(*)} callback
 * @this Set|Vector
 */
offObjectEvent: function (callback) {
    this._proxy.off(callback);
},

/**
 * Waits for collection to receive state from cache or uplink and then invokes passed callback
 *
 * @param {function()} callback
 * @this Set|Vector
...
```

#### <a name="apidoc.element.swarm.Vector.prototype._neutrals.on"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype._neutrals.</span>on (spec, filter, repl)](#apidoc.element.swarm.Vector.prototype._neutrals.on)
- description and source-code
```javascript
on = function (spec, filter, repl) {   // WELL  on() is not an op, right?
    // if no listener is supplied then the object is only
    // guaranteed to exist till the next Host.gc() run
    if (!repl) { return; }

    var self = this;
    // stateless objects fire no events; essentially, on() is deferred
    if (!this._version && filter) { // TODO solidify
        this._lstn.push({
            _op: 'reon',
            _src: repl,
            deliver: function () {
                var i = self._lstn.indexOf(this);
                self._lstn.splice(i, 1);
                self.deliver(spec, filter, repl);
            }
        });
        return; // defer this call till uplinks are ready
    }
    // make all listeners uniform objects
    if (repl.constructor === Function) {
        repl = {
            sink: repl,
            that: this,
            deliver: function () { // .deliver is invoked on an event
                this.sink.apply(this.that, arguments);
            }
        };
    }

    if (filter) {
        filter = new Spec(filter, '.');
        var baseVersion = filter.filter('!'),
            filter_by_op = filter.get('.');

        if (filter_by_op === 'init') {
            var diff_if_needed = baseVersion ? this.diff(baseVersion) : '';
            repl.deliver(spec.set('.init'), diff_if_needed, this); //??
            // FIXME use once()
            return;
        }
        if (filter_by_op) {
            repl = {
                sink: repl,
                _op: filter_by_op,
                deliver: function deliverWithFilter(spec, val, src) {
                    if (spec.op() === filter_by_op) {
                        this.sink.deliver(spec, val, src);
                    }
                }
            };
        }

        if (!baseVersion.isEmpty()) {
            var diff = this.diff(baseVersion);
            diff && repl.deliver(spec.set('.init'), diff, this); // 2downlink
            repl.deliver(spec.set('.reon'), this.version().toString(), this);
        }
    }

    this._lstn.push(repl);
    // TODO repeated subscriptions: send a diff, otherwise ignore
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.Vector.prototype._neutrals.reoff"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype._neutrals.</span>reoff (spec, val, repl)](#apidoc.element.swarm.Vector.prototype._neutrals.reoff)
- description and source-code
```javascript
reoff = function (spec, val, repl) {
    var idx = this.getListenerIndex(repl); //TODO ??? uplinks_only?
    if (idx > -1) {
        this._lstn.splice(idx, 1);
    }
    if (this._id) {
        this.checkUplink();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype._neutrals.reon"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype._neutrals.</span>reon (spec, filter, repl)](#apidoc.element.swarm.Vector.prototype._neutrals.reon)
- description and source-code
```javascript
reon = function (spec, filter, repl) {
    if (filter) {  // a diff is requested
        var base = Spec.as(filter).tok('!');
        var diff = this.diff(base);
        if (diff) {
            repl.deliver(spec.set('.init'), diff, this);
        }
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.Vector.prototype._ops"></a>[module swarm.Vector.prototype._ops](#apidoc.module.swarm.Vector.prototype._ops)

#### <a name="apidoc.element.swarm.Vector.prototype._ops.in"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype._ops.</span>in (spec, value, src)](#apidoc.element.swarm.Vector.prototype._ops.in)
- description and source-code
```javascript
in = function (spec, value, src) {
    // we misuse specifiers to express the operation in
    // a compact non-ambiguous way
    value = new Spec(value);
    var opid = spec.tok('!');
    var at = value.tok('!');
    if (opid<=at) {
        throw new Error('timestamps are messed up');
    }
    var what = value.tok('#');
    if (!what) { throw new Error('object #id not specified'); }
    var type = value.get('/');
    if (!type && this.objectType) {
        type = this.objectType.prototype._type;
    }
    if (!type) {
        throw new Error('object /type not specified');
    }
    type = '/' + type;

    var pos = this.findPositionFor(opid, at?at:'!0');
    var obj = this._host.get(type+what);

    this._objects.splice(pos.index,0,obj);
    this._order.insert(opid,pos);

    obj.on(this._proxy);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype._ops.init"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype._ops.</span>init (spec, state, src)](#apidoc.element.swarm.Vector.prototype._ops.init)
- description and source-code
```javascript
init = function (spec, state, src) {

    var tail = {}, // ops to be applied on top of the received state
        typeid = spec.filter('/#'),
        lstn = this._lstn,
        a_spec;
    this._lstn = []; // prevent events from being fired

    if (state._version/* && state._version !== '!0'*/) {
        // local changes may need to be merged into the received state
        if (this._oplog) {
            for (a_spec in this._oplog) {
                tail[a_spec] = this._oplog[a_spec];
            }
            this._oplog = {};
        }
        this._vector && (this._vector = undefined);
        // zero everything
        for (var key in this) {
            if (this.hasOwnProperty(key) && key.charAt(0) !== '_') {
                this[key] = undefined;
            }
        }
        // set default values
        this.reset();

        this.apply(state);
        this._version = state._version;

        state._oplog && (this._oplog = state._oplog); // FIXME copy
        state._vector && (this._vector = state._vector);
    }
    // add the received tail to the local one
    if (state._tail) {
        for (a_spec in state._tail) {
            tail[a_spec] = state._tail[a_spec];
        }
    }
    // appply the combined tail to the new state
    var specs = [];
    for (a_spec in tail) {
        specs.push(a_spec);
    }
    specs.sort().reverse();
    // there will be some replays, but those will be ignored
    while (a_spec = specs.pop()) {
        this.deliver(typeid.add(a_spec), tail[a_spec], this);
    }

    this._lstn = lstn;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.Vector.prototype._ops.rm"></a>[function <span class="apidocSignatureSpan">swarm.Vector.prototype._ops.</span>rm (spec, value, src)](#apidoc.element.swarm.Vector.prototype._ops.rm)
- description and source-code
```javascript
rm = function (spec, value, src) {
    value = Spec.as(value);
    var target = value.tok('!');
    var hint = value.has('.') ? Spec.base2int(value.get('.')) : 0;
    var at = this._order.find(target, Math.max(0,hint-5));
    if (at.end()) {
        at = this._order.find(target, 0);
    }
    if (at.end()) {
        // this can only be explained by concurrent deletion
        // partial order can't break cause-and-effect ordering
        return;
    }
    var obj = this._objects[at.index];
    this._objects.splice(at.index,1);
    at.erase(1);

    obj.off(this._proxy);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.WebSocketStream"></a>[module swarm.WebSocketStream](#apidoc.module.swarm.WebSocketStream)

#### <a name="apidoc.element.swarm.WebSocketStream.WebSocketStream"></a>[function <span class="apidocSignatureSpan">swarm.</span>WebSocketStream (url)](#apidoc.element.swarm.WebSocketStream.WebSocketStream)
- description and source-code
```javascript
function WebSocketStream(url) {
    var self = this;
    var ln = this.lstn = {};
    this.url = url;
    var ws = this.ws = new WebSocket(url);
    var buf = this.buf = [];
    ws.onopen = function () {
        buf.reverse();
        self.buf = null;
        while (buf.length) {
            self.write(buf.pop());
        }

    };
    ws.onclose = function () { ln.close && ln.close(); };
    ws.onmessage = function (msg) {
        ln.data && ln.data(msg.data);
    };
    ws.onerror = function (err) { ln.error && ln.error(err); };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.env"></a>[module swarm.env](#apidoc.module.swarm.env)

#### <a name="apidoc.element.swarm.env.hashfn"></a>[function <span class="apidocSignatureSpan">swarm.env.</span>hashfn (key, seed)](#apidoc.element.swarm.env.hashfn)
- description and source-code
```javascript
function murmurhash3_32_gc(key, seed) {
    var remainder, bytes, h1, h1b, c1, c2, k1, i;

    remainder = key.length & 3; // key.length % 4
    bytes = key.length - remainder;
    h1 = seed;
    c1 = 0xcc9e2d51;
    c2 = 0x1b873593;
    i = 0;

    while (i < bytes) {
        k1 =
                ((key.charCodeAt(i) & 0xff)) |
                ((key.charCodeAt(++i) & 0xff) << 8) |
                ((key.charCodeAt(++i) & 0xff) << 16) |
                ((key.charCodeAt(++i) & 0xff) << 24);
        ++i;

        k1 = ((((k1 & 0xffff) * c1) + ((((k1 >>> 16) * c1) & 0xffff) << 16))) & 0xffffffff;
        k1 = (k1 << 15) | (k1 >>> 17);
        k1 = ((((k1 & 0xffff) * c2) + ((((k1 >>> 16) * c2) & 0xffff) << 16))) & 0xffffffff;

        h1 ^= k1;
        h1 = (h1 << 13) | (h1 >>> 19);
        h1b = ((((h1 & 0xffff) * 5) + ((((h1 >>> 16) * 5) & 0xffff) << 16))) & 0xffffffff;
        h1 = (((h1b & 0xffff) + 0x6b64) + ((((h1b >>> 16) + 0xe654) & 0xffff) << 16));
    }

    k1 = 0;

    switch (remainder) {
    case 3:
        k1 ^= (key.charCodeAt(i + 2) & 0xff) << 16;
<span class="apidocCodeCommentSpan">        /* falls through */
</span>    case 2:
        k1 ^= (key.charCodeAt(i + 1) & 0xff) << 8;
        /* falls through */
    case 1:
        k1 ^= (key.charCodeAt(i) & 0xff);

        k1 = (((k1 & 0xffff) * c1) + ((((k1 >>> 16) * c1) & 0xffff) << 16)) & 0xffffffff;
        k1 = (k1 << 15) | (k1 >>> 17);
        k1 = (((k1 & 0xffff) * c2) + ((((k1 >>> 16) * c2) & 0xffff) << 16)) & 0xffffffff;
        h1 ^= k1;
    }

    h1 ^= key.length;

    h1 ^= h1 >>> 16;
    h1 = (((h1 & 0xffff) * 0x85ebca6b) + ((((h1 >>> 16) * 0x85ebca6b) & 0xffff) << 16)) & 0xffffffff;
    h1 ^= h1 >>> 13;
    h1 = ((((h1 & 0xffff) * 0xc2b2ae35) + ((((h1 >>> 16) * 0xc2b2ae35) & 0xffff) << 16))) & 0xffffffff;
    h1 ^= h1 >>> 16;

    return h1 >>> 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.env.log"></a>[function <span class="apidocSignatureSpan">swarm.env.</span>log (spec, val, object)](#apidoc.element.swarm.env.log)
- description and source-code
```javascript
function plain_log(spec, val, object) {
    var method = 'log';
    switch (spec.op()) {
    case 'error':
        method = 'error';
        break;
    case 'warn':
        method = 'warn';
        break;
    }
    console[method](spec.toString(), val, object && object._id,
            '@' + ((object && object._host && object._host._id) || ''));
}
```
- example usage
```shell
...
    mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
    // this will be triggered by every state change, be it
    // local or remote
    console.log('event: ', spec.op(), val);
    // outputs:
    // set {x:3, y:4}
});
'''

### Creating a simple NodeJS sync server
...
```



# <a name="apidoc.module.swarm.env.streams"></a>[module swarm.env.streams](#apidoc.module.swarm.env.streams)

#### <a name="apidoc.element.swarm.env.streams.loopback"></a>[function <span class="apidocSignatureSpan">swarm.env.streams.</span>loopback (url)](#apidoc.element.swarm.env.streams.loopback)
- description and source-code
```javascript
function AsyncLoopbackConnection(url) {
    var m = url.match(/loopback:(\w+)/);
    if (!m) {
        throw new Error('invalid url');
    }
    this.id = m[1];
    this.lstn = {};
    this.queue = [];
    if (this.id in AsyncLoopbackConnection.pipes) {
        throw new Error('duplicate');
    }
    AsyncLoopbackConnection.pipes[this.id] = this;
    var pair = this.pair();
    if (pair && pair.queue.length) {
        pair.write();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.env.streams.ws"></a>[function <span class="apidocSignatureSpan">swarm.env.streams.</span>ws (url)](#apidoc.element.swarm.env.streams.ws)
- description and source-code
```javascript
function WebSocketStream(url) {
    var self = this;
    var ln = this.lstn = {};
    this.url = url;
    var ws = this.ws = new WebSocket(url);
    var buf = this.buf = [];
    ws.onopen = function () {
        buf.reverse();
        self.buf = null;
        while (buf.length) {
            self.write(buf.pop());
        }

    };
    ws.onclose = function () { ln.close && ln.close(); };
    ws.onmessage = function (msg) {
        ln.data && ln.data(msg.data);
    };
    ws.onerror = function (err) { ln.error && ln.error(err); };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swarm.env.streams.wss"></a>[function <span class="apidocSignatureSpan">swarm.env.streams.</span>wss (url)](#apidoc.element.swarm.env.streams.wss)
- description and source-code
```javascript
function WebSocketStream(url) {
    var self = this;
    var ln = this.lstn = {};
    this.url = url;
    var ws = this.ws = new WebSocket(url);
    var buf = this.buf = [];
    ws.onopen = function () {
        buf.reverse();
        self.buf = null;
        while (buf.length) {
            self.write(buf.pop());
        }

    };
    ws.onclose = function () { ln.close && ln.close(); };
    ws.onmessage = function (msg) {
        ln.data && ln.data(msg.data);
    };
    ws.onerror = function (err) { ln.error && ln.error(err); };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swarm.env.streams.loopback.prototype"></a>[module swarm.env.streams.loopback.prototype](#apidoc.module.swarm.env.streams.loopback.prototype)

#### <a name="apidoc.element.swarm.env.streams.loopback.prototype.close"></a>[function <span class="apidocSignatureSpan">swarm.env.streams.loopback.prototype.</span>close ()](#apidoc.element.swarm.env.streams.loopback.prototype.close)
- description and source-code
```javascript
close = function () {
    delete AsyncLoopbackConnection.pipes[this.id];
    var pair = this.pair();
    pair && pair.close();
    this.lstn.close && this.lstn.close();
}
```
- example usage
```shell
...
        }
    }, 1);
};

AsyncLoopbackConnection.prototype.close = function () {
    delete AsyncLoopbackConnection.pipes[this.id];
    var pair = this.pair();
    pair && pair.close();
    this.lstn.close && this.lstn.close();
};
...
```

#### <a name="apidoc.element.swarm.env.streams.loopback.prototype.on"></a>[function <span class="apidocSignatureSpan">swarm.env.streams.loopback.prototype.</span>on (evname, fn)](#apidoc.element.swarm.env.streams.loopback.prototype.on)
- description and source-code
```javascript
on = function (evname, fn) {
    if (evname in this.lstn) {
        throw new Error('multiple listeners not supported');
    }
    this.lstn[evname] = fn;
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.env.streams.loopback.prototype.pair"></a>[function <span class="apidocSignatureSpan">swarm.env.streams.loopback.prototype.</span>pair ()](#apidoc.element.swarm.env.streams.loopback.prototype.pair)
- description and source-code
```javascript
pair = function () {
    var pairId = this.id.match(/./g).reverse().join('');
    return AsyncLoopbackConnection.pipes[pairId];
}
```
- example usage
```shell
...
    this.id = m[1];
    this.lstn = {};
    this.queue = [];
    if (this.id in AsyncLoopbackConnection.pipes) {
        throw new Error('duplicate');
    }
    AsyncLoopbackConnection.pipes[this.id] = this;
    var pair = this.pair();
    if (pair && pair.queue.length) {
        pair.write();
    }
}
AsyncLoopbackConnection.pipes = {};

env.streams.loopback = AsyncLoopbackConnection;
...
```

#### <a name="apidoc.element.swarm.env.streams.loopback.prototype.receive"></a>[function <span class="apidocSignatureSpan">swarm.env.streams.loopback.prototype.</span>receive (string)](#apidoc.element.swarm.env.streams.loopback.prototype.receive)
- description and source-code
```javascript
receive = function (string) {
    this.lstn.data && this.lstn.data(string);
}
```
- example usage
```shell
...
obj && self.queue.push(obj.toString());
setTimeout(function () {
    var pair = self.pair();
    if (!pair) {
        return;
    }
    while (self.queue.length) {
        pair.receive(self.queue.shift());
    }
}, 1);
};

AsyncLoopbackConnection.prototype.close = function () {
delete AsyncLoopbackConnection.pipes[this.id];
var pair = this.pair();
...
```

#### <a name="apidoc.element.swarm.env.streams.loopback.prototype.write"></a>[function <span class="apidocSignatureSpan">swarm.env.streams.loopback.prototype.</span>write (obj)](#apidoc.element.swarm.env.streams.loopback.prototype.write)
- description and source-code
```javascript
write = function (obj) {
    var self = this;
    obj && self.queue.push(obj.toString());
    setTimeout(function () {
        var pair = self.pair();
        if (!pair) {
            return;
        }
        while (self.queue.length) {
            pair.receive(self.queue.shift());
        }
    }, 1);
}
```
- example usage
```shell
...
    this.queue = [];
    if (this.id in AsyncLoopbackConnection.pipes) {
        throw new Error('duplicate');
    }
    AsyncLoopbackConnection.pipes[this.id] = this;
    var pair = this.pair();
    if (pair && pair.queue.length) {
        pair.write();
    }
}
AsyncLoopbackConnection.pipes = {};

env.streams.loopback = AsyncLoopbackConnection;

AsyncLoopbackConnection.prototype.pair = function () {
...
```



# <a name="apidoc.module.swarm.env.streams.wss.prototype"></a>[module swarm.env.streams.wss.prototype](#apidoc.module.swarm.env.streams.wss.prototype)

#### <a name="apidoc.element.swarm.env.streams.wss.prototype.on"></a>[function <span class="apidocSignatureSpan">swarm.env.streams.wss.prototype.</span>on (evname, fn)](#apidoc.element.swarm.env.streams.wss.prototype.on)
- description and source-code
```javascript
on = function (evname, fn) {
    if (evname in this.lstn) {
        var self = this,
            prev_fn = this.lstn[evname];
        this.lstn[evname] = function () {
            prev_fn.apply(self, arguments);
            fn.apply(self, arguments);
        };
    } else {
        this.lstn[evname] = fn;
    }
}
```
- example usage
```shell
...
someMouse.set({x:1,y:2});

// 3.b. This object is global (we supply a certain id) so we
// may need to wait for its state to arrive from the server
var mickey = new Mouse('Mickey');

// 4.b. ...wait for the state to arrive
mickey.on('init', function () {
// ...so we may touch it finally.
mickey.set({x: 3, y: 4});
});

// 5. let's subscribe to the object's change events
mickey.on(function (spec, val, source) {
// this will be triggered by every state change, be it
...
```

#### <a name="apidoc.element.swarm.env.streams.wss.prototype.write"></a>[function <span class="apidocSignatureSpan">swarm.env.streams.wss.prototype.</span>write (data)](#apidoc.element.swarm.env.streams.wss.prototype.write)
- description and source-code
```javascript
write = function (data) {
    if (this.buf) {
        this.buf.push(data);
    } else {
        this.ws.send(data);
    }
}
```
- example usage
```shell
...
    this.queue = [];
    if (this.id in AsyncLoopbackConnection.pipes) {
        throw new Error('duplicate');
    }
    AsyncLoopbackConnection.pipes[this.id] = this;
    var pair = this.pair();
    if (pair && pair.queue.length) {
        pair.write();
    }
}
AsyncLoopbackConnection.pipes = {};

env.streams.loopback = AsyncLoopbackConnection;

AsyncLoopbackConnection.prototype.pair = function () {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
