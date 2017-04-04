# api documentation for  [xpath (v0.0.24)](https://github.com/goto100/xpath#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-xpath.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-xpath) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-xpath.svg)](https://travis-ci.org/npmdoc/node-npmdoc-xpath)
#### DOM 3 XPath implemention and helper for node.js.

[![NPM](https://nodei.co/npm/xpath.png?downloads=true)](https://www.npmjs.com/package/xpath)

[![apidoc](https://npmdoc.github.io/node-npmdoc-xpath/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-xpath_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-xpath/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-xpath/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-xpath/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Cameron McCormac"
    },
    "bugs": {
        "url": "https://github.com/goto100/xpath/issues"
    },
    "contributors": [
        {
            "name": "goto100"
        },
        {
            "name": "James Rishe"
        }
    ],
    "dependencies": {},
    "description": "DOM 3 XPath implemention and helper for node.js.",
    "devDependencies": {
        "nodeunit": ">=0.6.4",
        "xmldom": "^0.1.19"
    },
    "directories": {},
    "dist": {
        "shasum": "1ade162e1cc523c8d39fc7d06afc16ea216f29fb",
        "tarball": "https://registry.npmjs.org/xpath/-/xpath-0.0.24.tgz"
    },
    "engines": {
        "node": ">=0.6.0"
    },
    "gitHead": "6e7c0b68d9e268699f837c392c2b102225a5cf5a",
    "homepage": "https://github.com/goto100/xpath#readme",
    "keywords": [
        "xpath",
        "xml"
    ],
    "license": "CC-BY-SA-2.0",
    "main": "./xpath.js",
    "maintainers": [
        {
            "name": "goto100",
            "email": "goto100@gmail.com"
        },
        {
            "name": "jlrishe",
            "email": "jrishe@gmail.com"
        }
    ],
    "name": "xpath",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/goto100/xpath.git"
    },
    "scripts": {
        "test": "nodeunit test.js"
    },
    "typings": "./xpath.d.ts",
    "version": "0.0.24"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module xpath](#apidoc.module.xpath)
1.  [function <span class="apidocSignatureSpan">xpath.</span>BarOperation (lhs, rhs)](#apidoc.element.xpath.BarOperation)
1.  [function <span class="apidocSignatureSpan">xpath.</span>FunctionResolver (thisArg)](#apidoc.element.xpath.FunctionResolver)
1.  [function <span class="apidocSignatureSpan">xpath.</span>NamespaceResolver ()](#apidoc.element.xpath.NamespaceResolver)
1.  [function <span class="apidocSignatureSpan">xpath.</span>NodeTest (type, value)](#apidoc.element.xpath.NodeTest)
1.  [function <span class="apidocSignatureSpan">xpath.</span>Step (axis, nodetest, preds)](#apidoc.element.xpath.Step)
1.  [function <span class="apidocSignatureSpan">xpath.</span>VariableResolver ()](#apidoc.element.xpath.VariableResolver)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XBoolean (b)](#apidoc.element.xpath.XBoolean)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XNodeSet ()](#apidoc.element.xpath.XNodeSet)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XNumber (n)](#apidoc.element.xpath.XNumber)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XPath (e)](#apidoc.element.xpath.XPath)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XPathContext (vr, nr, fr)](#apidoc.element.xpath.XPathContext)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XPathParser ()](#apidoc.element.xpath.XPathParser)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XPathResult (v, t)](#apidoc.element.xpath.XPathResult)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XString (s)](#apidoc.element.xpath.XString)
1.  [function <span class="apidocSignatureSpan">xpath.</span>createExpression (e, r)](#apidoc.element.xpath.createExpression)
1.  [function <span class="apidocSignatureSpan">xpath.</span>createNSResolver (n)](#apidoc.element.xpath.createNSResolver)
1.  [function <span class="apidocSignatureSpan">xpath.</span>evaluate (e, cn, r, t, res)](#apidoc.element.xpath.evaluate)
1.  [function <span class="apidocSignatureSpan">xpath.</span>parse (xpath)](#apidoc.element.xpath.parse)
1.  [function <span class="apidocSignatureSpan">xpath.</span>select (e, doc, single)](#apidoc.element.xpath.select)
1.  [function <span class="apidocSignatureSpan">xpath.</span>select1 (e, doc)](#apidoc.element.xpath.select1)
1.  [function <span class="apidocSignatureSpan">xpath.</span>selectWithResolver (e, doc, resolver, single)](#apidoc.element.xpath.selectWithResolver)
1.  [function <span class="apidocSignatureSpan">xpath.</span>useNamespaces (mappings)](#apidoc.element.xpath.useNamespaces)
1.  object <span class="apidocSignatureSpan">xpath.</span>BarOperation.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>BarOperation.superclass
1.  object <span class="apidocSignatureSpan">xpath.</span>FunctionResolver.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>NamespaceResolver.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>NodeTest.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>Step.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>Utilities
1.  object <span class="apidocSignatureSpan">xpath.</span>VariableResolver.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>XBoolean.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>XBoolean.superclass
1.  object <span class="apidocSignatureSpan">xpath.</span>XNodeSet.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>XNumber.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>XPath.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>XPathContext.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>XPathParser.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>XPathResult.prototype
1.  object <span class="apidocSignatureSpan">xpath.</span>XString.prototype

#### [module xpath.BarOperation](#apidoc.module.xpath.BarOperation)
1.  [function <span class="apidocSignatureSpan">xpath.</span>BarOperation (lhs, rhs)](#apidoc.element.xpath.BarOperation.BarOperation)
1.  object <span class="apidocSignatureSpan">xpath.BarOperation.</span>superclass

#### [module xpath.BarOperation.prototype](#apidoc.module.xpath.BarOperation.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.BarOperation.prototype.</span>constructor (lhs, rhs)](#apidoc.element.xpath.BarOperation.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.BarOperation.prototype.</span>evaluate (c)](#apidoc.element.xpath.BarOperation.prototype.evaluate)
1.  [function <span class="apidocSignatureSpan">xpath.BarOperation.prototype.</span>init (lhs, rhs)](#apidoc.element.xpath.BarOperation.prototype.init)
1.  [function <span class="apidocSignatureSpan">xpath.BarOperation.prototype.</span>toString ()](#apidoc.element.xpath.BarOperation.prototype.toString)

#### [module xpath.BarOperation.superclass](#apidoc.module.xpath.BarOperation.superclass)
1.  [function <span class="apidocSignatureSpan">xpath.BarOperation.superclass.</span>constructor (lhs, rhs)](#apidoc.element.xpath.BarOperation.superclass.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.BarOperation.superclass.</span>init (lhs, rhs)](#apidoc.element.xpath.BarOperation.superclass.init)

#### [module xpath.FunctionResolver](#apidoc.module.xpath.FunctionResolver)
1.  [function <span class="apidocSignatureSpan">xpath.</span>FunctionResolver (thisArg)](#apidoc.element.xpath.FunctionResolver.FunctionResolver)
1.  [function <span class="apidocSignatureSpan">xpath.FunctionResolver.</span>getFunctionFromContext (qName, context)](#apidoc.element.xpath.FunctionResolver.getFunctionFromContext)
1.  object <span class="apidocSignatureSpan">xpath.FunctionResolver.</span>superclass

#### [module xpath.FunctionResolver.prototype](#apidoc.module.xpath.FunctionResolver.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.FunctionResolver.prototype.</span>addFunction (ns, ln, f)](#apidoc.element.xpath.FunctionResolver.prototype.addFunction)
1.  [function <span class="apidocSignatureSpan">xpath.FunctionResolver.prototype.</span>addStandardFunctions ()](#apidoc.element.xpath.FunctionResolver.prototype.addStandardFunctions)
1.  [function <span class="apidocSignatureSpan">xpath.FunctionResolver.prototype.</span>constructor (thisArg)](#apidoc.element.xpath.FunctionResolver.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.FunctionResolver.prototype.</span>getFunction (localName, namespace)](#apidoc.element.xpath.FunctionResolver.prototype.getFunction)

#### [module xpath.NamespaceResolver](#apidoc.module.xpath.NamespaceResolver)
1.  [function <span class="apidocSignatureSpan">xpath.</span>NamespaceResolver ()](#apidoc.element.xpath.NamespaceResolver.NamespaceResolver)
1.  object <span class="apidocSignatureSpan">xpath.NamespaceResolver.</span>superclass

#### [module xpath.NamespaceResolver.prototype](#apidoc.module.xpath.NamespaceResolver.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.NamespaceResolver.prototype.</span>constructor ()](#apidoc.element.xpath.NamespaceResolver.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.NamespaceResolver.prototype.</span>getNamespace (prefix, n)](#apidoc.element.xpath.NamespaceResolver.prototype.getNamespace)

#### [module xpath.NodeTest](#apidoc.module.xpath.NodeTest)
1.  [function <span class="apidocSignatureSpan">xpath.</span>NodeTest (type, value)](#apidoc.element.xpath.NodeTest.NodeTest)
1.  number <span class="apidocSignatureSpan">xpath.NodeTest.</span>COMMENT
1.  number <span class="apidocSignatureSpan">xpath.NodeTest.</span>NAMETESTANY
1.  number <span class="apidocSignatureSpan">xpath.NodeTest.</span>NAMETESTPREFIXANY
1.  number <span class="apidocSignatureSpan">xpath.NodeTest.</span>NAMETESTQNAME
1.  number <span class="apidocSignatureSpan">xpath.NodeTest.</span>NODE
1.  number <span class="apidocSignatureSpan">xpath.NodeTest.</span>PI
1.  number <span class="apidocSignatureSpan">xpath.NodeTest.</span>TEXT
1.  object <span class="apidocSignatureSpan">xpath.NodeTest.</span>superclass

#### [module xpath.NodeTest.prototype](#apidoc.module.xpath.NodeTest.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.NodeTest.prototype.</span>constructor (type, value)](#apidoc.element.xpath.NodeTest.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.NodeTest.prototype.</span>init (type, value)](#apidoc.element.xpath.NodeTest.prototype.init)
1.  [function <span class="apidocSignatureSpan">xpath.NodeTest.prototype.</span>matches (n, xpc)](#apidoc.element.xpath.NodeTest.prototype.matches)
1.  [function <span class="apidocSignatureSpan">xpath.NodeTest.prototype.</span>toString ()](#apidoc.element.xpath.NodeTest.prototype.toString)

#### [module xpath.Step](#apidoc.module.xpath.Step)
1.  [function <span class="apidocSignatureSpan">xpath.</span>Step (axis, nodetest, preds)](#apidoc.element.xpath.Step.Step)
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>ANCESTOR
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>ANCESTORORSELF
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>ATTRIBUTE
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>CHILD
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>DESCENDANT
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>DESCENDANTORSELF
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>FOLLOWING
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>FOLLOWINGSIBLING
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>NAMESPACE
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>PARENT
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>PRECEDING
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>PRECEDINGSIBLING
1.  number <span class="apidocSignatureSpan">xpath.Step.</span>SELF
1.  object <span class="apidocSignatureSpan">xpath.Step.</span>superclass

#### [module xpath.Step.prototype](#apidoc.module.xpath.Step.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.Step.prototype.</span>constructor (axis, nodetest, preds)](#apidoc.element.xpath.Step.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.Step.prototype.</span>init (axis, nodetest, preds)](#apidoc.element.xpath.Step.prototype.init)
1.  [function <span class="apidocSignatureSpan">xpath.Step.prototype.</span>toString ()](#apidoc.element.xpath.Step.prototype.toString)

#### [module xpath.Utilities](#apidoc.module.xpath.Utilities)
1.  [function <span class="apidocSignatureSpan">xpath.Utilities.</span>coalesceText (n)](#apidoc.element.xpath.Utilities.coalesceText)
1.  [function <span class="apidocSignatureSpan">xpath.Utilities.</span>getElementById (n, id)](#apidoc.element.xpath.Utilities.getElementById)
1.  [function <span class="apidocSignatureSpan">xpath.Utilities.</span>instance_of (o, c)](#apidoc.element.xpath.Utilities.instance_of)
1.  [function <span class="apidocSignatureSpan">xpath.Utilities.</span>isAttribute (val)](#apidoc.element.xpath.Utilities.isAttribute)
1.  [function <span class="apidocSignatureSpan">xpath.Utilities.</span>isLetter (c)](#apidoc.element.xpath.Utilities.isLetter)
1.  [function <span class="apidocSignatureSpan">xpath.Utilities.</span>isNCNameChar (c)](#apidoc.element.xpath.Utilities.isNCNameChar)
1.  [function <span class="apidocSignatureSpan">xpath.Utilities.</span>isSpace (c)](#apidoc.element.xpath.Utilities.isSpace)
1.  [function <span class="apidocSignatureSpan">xpath.Utilities.</span>resolveQName (qn, nr, n, useDefault)](#apidoc.element.xpath.Utilities.resolveQName)
1.  [function <span class="apidocSignatureSpan">xpath.Utilities.</span>splitQName (qn)](#apidoc.element.xpath.Utilities.splitQName)

#### [module xpath.VariableResolver](#apidoc.module.xpath.VariableResolver)
1.  [function <span class="apidocSignatureSpan">xpath.</span>VariableResolver ()](#apidoc.element.xpath.VariableResolver.VariableResolver)
1.  object <span class="apidocSignatureSpan">xpath.VariableResolver.</span>superclass

#### [module xpath.VariableResolver.prototype](#apidoc.module.xpath.VariableResolver.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.VariableResolver.prototype.</span>constructor ()](#apidoc.element.xpath.VariableResolver.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.VariableResolver.prototype.</span>getVariable (ln, ns)](#apidoc.element.xpath.VariableResolver.prototype.getVariable)

#### [module xpath.XBoolean](#apidoc.module.xpath.XBoolean)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XBoolean (b)](#apidoc.element.xpath.XBoolean.XBoolean)
1.  object <span class="apidocSignatureSpan">xpath.XBoolean.</span>superclass

#### [module xpath.XBoolean.prototype](#apidoc.module.xpath.XBoolean.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>bool ()](#apidoc.element.xpath.XBoolean.prototype.bool)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>booleanValue ()](#apidoc.element.xpath.XBoolean.prototype.booleanValue)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>constructor (b)](#apidoc.element.xpath.XBoolean.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>equals (r)](#apidoc.element.xpath.XBoolean.prototype.equals)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>evaluate (c)](#apidoc.element.xpath.XBoolean.prototype.evaluate)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>greaterthan (r)](#apidoc.element.xpath.XBoolean.prototype.greaterthan)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>greaterthanorequal (r)](#apidoc.element.xpath.XBoolean.prototype.greaterthanorequal)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>init (b)](#apidoc.element.xpath.XBoolean.prototype.init)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>lessthan (r)](#apidoc.element.xpath.XBoolean.prototype.lessthan)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>lessthanorequal (r)](#apidoc.element.xpath.XBoolean.prototype.lessthanorequal)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>nodeset ()](#apidoc.element.xpath.XBoolean.prototype.nodeset)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>not ()](#apidoc.element.xpath.XBoolean.prototype.not)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>notequal (r)](#apidoc.element.xpath.XBoolean.prototype.notequal)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>number ()](#apidoc.element.xpath.XBoolean.prototype.number)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>numberValue ()](#apidoc.element.xpath.XBoolean.prototype.numberValue)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>string ()](#apidoc.element.xpath.XBoolean.prototype.string)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>stringValue ()](#apidoc.element.xpath.XBoolean.prototype.stringValue)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>toString ()](#apidoc.element.xpath.XBoolean.prototype.toString)

#### [module xpath.XBoolean.superclass](#apidoc.module.xpath.XBoolean.superclass)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.superclass.</span>constructor ()](#apidoc.element.xpath.XBoolean.superclass.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.superclass.</span>evaluate (c)](#apidoc.element.xpath.XBoolean.superclass.evaluate)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.superclass.</span>init ()](#apidoc.element.xpath.XBoolean.superclass.init)
1.  [function <span class="apidocSignatureSpan">xpath.XBoolean.superclass.</span>toString ()](#apidoc.element.xpath.XBoolean.superclass.toString)

#### [module xpath.XNodeSet](#apidoc.module.xpath.XNodeSet)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XNodeSet ()](#apidoc.element.xpath.XNodeSet.XNodeSet)
1.  object <span class="apidocSignatureSpan">xpath.XNodeSet.</span>superclass

#### [module xpath.XNodeSet.prototype](#apidoc.module.xpath.XNodeSet.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>add (n)](#apidoc.element.xpath.XNodeSet.prototype.add)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>addArray (ns)](#apidoc.element.xpath.XNodeSet.prototype.addArray)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>bool ()](#apidoc.element.xpath.XNodeSet.prototype.bool)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>booleanValue ()](#apidoc.element.xpath.XNodeSet.prototype.booleanValue)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>buildTree ()](#apidoc.element.xpath.XNodeSet.prototype.buildTree)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>compareWithBoolean (r, o)](#apidoc.element.xpath.XNodeSet.prototype.compareWithBoolean)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>compareWithNodeSet (r, o)](#apidoc.element.xpath.XNodeSet.prototype.compareWithNodeSet)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>compareWithNumber (r, o)](#apidoc.element.xpath.XNodeSet.prototype.compareWithNumber)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>compareWithString (r, o)](#apidoc.element.xpath.XNodeSet.prototype.compareWithString)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>constructor ()](#apidoc.element.xpath.XNodeSet.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>equals (r)](#apidoc.element.xpath.XNodeSet.prototype.equals)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>evaluate (c)](#apidoc.element.xpath.XNodeSet.prototype.evaluate)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>first ()](#apidoc.element.xpath.XNodeSet.prototype.first)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>greaterthan (r)](#apidoc.element.xpath.XNodeSet.prototype.greaterthan)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>greaterthanorequal (r)](#apidoc.element.xpath.XNodeSet.prototype.greaterthanorequal)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>init ()](#apidoc.element.xpath.XNodeSet.prototype.init)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>lessthan (r)](#apidoc.element.xpath.XNodeSet.prototype.lessthan)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>lessthanorequal (r)](#apidoc.element.xpath.XNodeSet.prototype.lessthanorequal)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>nodeset ()](#apidoc.element.xpath.XNodeSet.prototype.nodeset)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>notequal (r)](#apidoc.element.xpath.XNodeSet.prototype.notequal)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>number ()](#apidoc.element.xpath.XNodeSet.prototype.number)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>numberValue ()](#apidoc.element.xpath.XNodeSet.prototype.numberValue)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>string ()](#apidoc.element.xpath.XNodeSet.prototype.string)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>stringForContainerNode (n)](#apidoc.element.xpath.XNodeSet.prototype.stringForContainerNode)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>stringForNode (n)](#apidoc.element.xpath.XNodeSet.prototype.stringForNode)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>stringValue ()](#apidoc.element.xpath.XNodeSet.prototype.stringValue)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>toArray ()](#apidoc.element.xpath.XNodeSet.prototype.toArray)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>toArrayRec (t, a)](#apidoc.element.xpath.XNodeSet.prototype.toArrayRec)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>toString ()](#apidoc.element.xpath.XNodeSet.prototype.toString)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>toUnsortedArray ()](#apidoc.element.xpath.XNodeSet.prototype.toUnsortedArray)
1.  [function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>union (r)](#apidoc.element.xpath.XNodeSet.prototype.union)

#### [module xpath.XNumber](#apidoc.module.xpath.XNumber)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XNumber (n)](#apidoc.element.xpath.XNumber.XNumber)
1.  object <span class="apidocSignatureSpan">xpath.XNumber.</span>superclass

#### [module xpath.XNumber.prototype](#apidoc.module.xpath.XNumber.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>bool ()](#apidoc.element.xpath.XNumber.prototype.bool)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>booleanValue ()](#apidoc.element.xpath.XNumber.prototype.booleanValue)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>constructor (n)](#apidoc.element.xpath.XNumber.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>div (r)](#apidoc.element.xpath.XNumber.prototype.div)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>equals (r)](#apidoc.element.xpath.XNumber.prototype.equals)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>evaluate (c)](#apidoc.element.xpath.XNumber.prototype.evaluate)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>greaterthan (r)](#apidoc.element.xpath.XNumber.prototype.greaterthan)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>greaterthanorequal (r)](#apidoc.element.xpath.XNumber.prototype.greaterthanorequal)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>init (n)](#apidoc.element.xpath.XNumber.prototype.init)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>lessthan (r)](#apidoc.element.xpath.XNumber.prototype.lessthan)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>lessthanorequal (r)](#apidoc.element.xpath.XNumber.prototype.lessthanorequal)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>minus (r)](#apidoc.element.xpath.XNumber.prototype.minus)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>mod (r)](#apidoc.element.xpath.XNumber.prototype.mod)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>multiply (r)](#apidoc.element.xpath.XNumber.prototype.multiply)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>negate ()](#apidoc.element.xpath.XNumber.prototype.negate)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>nodeset ()](#apidoc.element.xpath.XNumber.prototype.nodeset)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>notequal (r)](#apidoc.element.xpath.XNumber.prototype.notequal)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>number ()](#apidoc.element.xpath.XNumber.prototype.number)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>numberValue ()](#apidoc.element.xpath.XNumber.prototype.numberValue)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>parse (s)](#apidoc.element.xpath.XNumber.prototype.parse)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>plus (r)](#apidoc.element.xpath.XNumber.prototype.plus)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>string ()](#apidoc.element.xpath.XNumber.prototype.string)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>stringValue ()](#apidoc.element.xpath.XNumber.prototype.stringValue)
1.  [function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>toString ()](#apidoc.element.xpath.XNumber.prototype.toString)
1.  object <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>numberFormat

#### [module xpath.XPath](#apidoc.module.xpath.XPath)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XPath (e)](#apidoc.element.xpath.XPath.XPath)
1.  object <span class="apidocSignatureSpan">xpath.XPath.</span>superclass
1.  string <span class="apidocSignatureSpan">xpath.XPath.</span>XMLNS_NAMESPACE_URI
1.  string <span class="apidocSignatureSpan">xpath.XPath.</span>XML_NAMESPACE_URI

#### [module xpath.XPath.prototype](#apidoc.module.xpath.XPath.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.XPath.prototype.</span>constructor (e)](#apidoc.element.xpath.XPath.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.XPath.prototype.</span>evaluate (c)](#apidoc.element.xpath.XPath.prototype.evaluate)
1.  [function <span class="apidocSignatureSpan">xpath.XPath.prototype.</span>toString ()](#apidoc.element.xpath.XPath.prototype.toString)

#### [module xpath.XPathContext](#apidoc.module.xpath.XPathContext)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XPathContext (vr, nr, fr)](#apidoc.element.xpath.XPathContext.XPathContext)
1.  object <span class="apidocSignatureSpan">xpath.XPathContext.</span>superclass

#### [module xpath.XPathContext.prototype](#apidoc.module.xpath.XPathContext.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.XPathContext.prototype.</span>constructor (vr, nr, fr)](#apidoc.element.xpath.XPathContext.prototype.constructor)

#### [module xpath.XPathParser](#apidoc.module.xpath.XPathParser)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XPathParser ()](#apidoc.element.xpath.XPathParser.XPathParser)
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>AND
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>ASTERISKNAMETEST
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>AT
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>AXISNAME
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>BAR
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>COMMA
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>DIV
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>DOLLAR
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>DOT
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>DOUBLECOLON
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>DOUBLEDOT
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>DOUBLESLASH
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>EQUALS
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>FUNCTIONNAME
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>GREATERTHAN
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>GREATERTHANOREQUAL
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>LEFTBRACKET
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>LEFTPARENTHESIS
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>LESSTHAN
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>LESSTHANOREQUAL
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>LITERAL
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>MINUS
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>MOD
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>MULTIPLYOPERATOR
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>NCNAMECOLONASTERISK
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>NODETYPE
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>NOTEQUAL
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>NUMBER
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>OR
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>PLUS
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>PROCESSINGINSTRUCTIONWITHLITERAL
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>QNAME
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>RIGHTBRACKET
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>RIGHTPARENTHESIS
1.  number <span class="apidocSignatureSpan">xpath.XPathParser.</span>SLASH
1.  object <span class="apidocSignatureSpan">xpath.XPathParser.</span>actionTable
1.  object <span class="apidocSignatureSpan">xpath.XPathParser.</span>actionTableNumber
1.  object <span class="apidocSignatureSpan">xpath.XPathParser.</span>gotoTable
1.  object <span class="apidocSignatureSpan">xpath.XPathParser.</span>productions
1.  object <span class="apidocSignatureSpan">xpath.XPathParser.</span>superclass
1.  string <span class="apidocSignatureSpan">xpath.XPathParser.</span>ACCEPT
1.  string <span class="apidocSignatureSpan">xpath.XPathParser.</span>REDUCE
1.  string <span class="apidocSignatureSpan">xpath.XPathParser.</span>SHIFT

#### [module xpath.XPathParser.prototype](#apidoc.module.xpath.XPathParser.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.XPathParser.prototype.</span>constructor ()](#apidoc.element.xpath.XPathParser.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.XPathParser.prototype.</span>init ()](#apidoc.element.xpath.XPathParser.prototype.init)
1.  [function <span class="apidocSignatureSpan">xpath.XPathParser.prototype.</span>parse (s)](#apidoc.element.xpath.XPathParser.prototype.parse)
1.  [function <span class="apidocSignatureSpan">xpath.XPathParser.prototype.</span>tokenize (s1)](#apidoc.element.xpath.XPathParser.prototype.tokenize)

#### [module xpath.XPathResult](#apidoc.module.xpath.XPathResult)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XPathResult (v, t)](#apidoc.element.xpath.XPathResult.XPathResult)
1.  number <span class="apidocSignatureSpan">xpath.XPathResult.</span>ANY_TYPE
1.  number <span class="apidocSignatureSpan">xpath.XPathResult.</span>ANY_UNORDERED_NODE_TYPE
1.  number <span class="apidocSignatureSpan">xpath.XPathResult.</span>BOOLEAN_TYPE
1.  number <span class="apidocSignatureSpan">xpath.XPathResult.</span>FIRST_ORDERED_NODE_TYPE
1.  number <span class="apidocSignatureSpan">xpath.XPathResult.</span>NUMBER_TYPE
1.  number <span class="apidocSignatureSpan">xpath.XPathResult.</span>ORDERED_NODE_ITERATOR_TYPE
1.  number <span class="apidocSignatureSpan">xpath.XPathResult.</span>ORDERED_NODE_SNAPSHOT_TYPE
1.  number <span class="apidocSignatureSpan">xpath.XPathResult.</span>STRING_TYPE
1.  number <span class="apidocSignatureSpan">xpath.XPathResult.</span>UNORDERED_NODE_ITERATOR_TYPE
1.  number <span class="apidocSignatureSpan">xpath.XPathResult.</span>UNORDERED_NODE_SNAPSHOT_TYPE
1.  object <span class="apidocSignatureSpan">xpath.XPathResult.</span>superclass

#### [module xpath.XPathResult.prototype](#apidoc.module.xpath.XPathResult.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.XPathResult.prototype.</span>constructor (v, t)](#apidoc.element.xpath.XPathResult.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.XPathResult.prototype.</span>iterateNext ()](#apidoc.element.xpath.XPathResult.prototype.iterateNext)
1.  [function <span class="apidocSignatureSpan">xpath.XPathResult.prototype.</span>snapshotItem (i)](#apidoc.element.xpath.XPathResult.prototype.snapshotItem)

#### [module xpath.XString](#apidoc.module.xpath.XString)
1.  [function <span class="apidocSignatureSpan">xpath.</span>XString (s)](#apidoc.element.xpath.XString.XString)
1.  object <span class="apidocSignatureSpan">xpath.XString.</span>superclass

#### [module xpath.XString.prototype](#apidoc.module.xpath.XString.prototype)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>bool ()](#apidoc.element.xpath.XString.prototype.bool)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>booleanValue ()](#apidoc.element.xpath.XString.prototype.booleanValue)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>constructor (s)](#apidoc.element.xpath.XString.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>equals (r)](#apidoc.element.xpath.XString.prototype.equals)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>evaluate (c)](#apidoc.element.xpath.XString.prototype.evaluate)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>greaterthan (r)](#apidoc.element.xpath.XString.prototype.greaterthan)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>greaterthanorequal (r)](#apidoc.element.xpath.XString.prototype.greaterthanorequal)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>init (s)](#apidoc.element.xpath.XString.prototype.init)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>lessthan (r)](#apidoc.element.xpath.XString.prototype.lessthan)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>lessthanorequal (r)](#apidoc.element.xpath.XString.prototype.lessthanorequal)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>nodeset ()](#apidoc.element.xpath.XString.prototype.nodeset)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>notequal (r)](#apidoc.element.xpath.XString.prototype.notequal)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>number ()](#apidoc.element.xpath.XString.prototype.number)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>numberValue ()](#apidoc.element.xpath.XString.prototype.numberValue)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>string ()](#apidoc.element.xpath.XString.prototype.string)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>stringValue ()](#apidoc.element.xpath.XString.prototype.stringValue)
1.  [function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>toString ()](#apidoc.element.xpath.XString.prototype.toString)



# <a name="apidoc.module.xpath"></a>[module xpath](#apidoc.module.xpath)

#### <a name="apidoc.element.xpath.BarOperation"></a>[function <span class="apidocSignatureSpan">xpath.</span>BarOperation (lhs, rhs)](#apidoc.element.xpath.BarOperation)
- description and source-code
```javascript
function BarOperation(lhs, rhs) {
	if (arguments.length > 0) {
		this.init(lhs, rhs);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.FunctionResolver"></a>[function <span class="apidocSignatureSpan">xpath.</span>FunctionResolver (thisArg)](#apidoc.element.xpath.FunctionResolver)
- description and source-code
```javascript
function FunctionResolver(thisArg) {
	this.thisArg = thisArg != null ? thisArg : Functions;
	this.functions = new Object();
	this.addStandardFunctions();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.NamespaceResolver"></a>[function <span class="apidocSignatureSpan">xpath.</span>NamespaceResolver ()](#apidoc.element.xpath.NamespaceResolver)
- description and source-code
```javascript
function NamespaceResolver() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.NodeTest"></a>[function <span class="apidocSignatureSpan">xpath.</span>NodeTest (type, value)](#apidoc.element.xpath.NodeTest)
- description and source-code
```javascript
function NodeTest(type, value) {
	if (arguments.length > 0) {
		this.init(type, value);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.Step"></a>[function <span class="apidocSignatureSpan">xpath.</span>Step (axis, nodetest, preds)](#apidoc.element.xpath.Step)
- description and source-code
```javascript
function Step(axis, nodetest, preds) {
	if (arguments.length > 0) {
		this.init(axis, nodetest, preds);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.VariableResolver"></a>[function <span class="apidocSignatureSpan">xpath.</span>VariableResolver ()](#apidoc.element.xpath.VariableResolver)
- description and source-code
```javascript
function VariableResolver() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean"></a>[function <span class="apidocSignatureSpan">xpath.</span>XBoolean (b)](#apidoc.element.xpath.XBoolean)
- description and source-code
```javascript
function XBoolean(b) {
	if (arguments.length > 0) {
		this.init(b);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet"></a>[function <span class="apidocSignatureSpan">xpath.</span>XNodeSet ()](#apidoc.element.xpath.XNodeSet)
- description and source-code
```javascript
function XNodeSet() {
	this.init();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber"></a>[function <span class="apidocSignatureSpan">xpath.</span>XNumber (n)](#apidoc.element.xpath.XNumber)
- description and source-code
```javascript
function XNumber(n) {
	if (arguments.length > 0) {
		this.init(n);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XPath"></a>[function <span class="apidocSignatureSpan">xpath.</span>XPath (e)](#apidoc.element.xpath.XPath)
- description and source-code
```javascript
function XPath(e) {
	this.expression = e;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XPathContext"></a>[function <span class="apidocSignatureSpan">xpath.</span>XPathContext (vr, nr, fr)](#apidoc.element.xpath.XPathContext)
- description and source-code
```javascript
function XPathContext(vr, nr, fr) {
	this.variableResolver = vr != null ? vr : new VariableResolver();
	this.namespaceResolver = nr != null ? nr : new NamespaceResolver();
	this.functionResolver = fr != null ? fr : new FunctionResolver();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XPathParser"></a>[function <span class="apidocSignatureSpan">xpath.</span>XPathParser ()](#apidoc.element.xpath.XPathParser)
- description and source-code
```javascript
function XPathParser() {
	this.init();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XPathResult"></a>[function <span class="apidocSignatureSpan">xpath.</span>XPathResult (v, t)](#apidoc.element.xpath.XPathResult)
- description and source-code
```javascript
function XPathResult(v, t) {
	if (t == XPathResult.ANY_TYPE) {
		if (v.constructor === XString) {
			t = XPathResult.STRING_TYPE;
		} else if (v.constructor === XNumber) {
			t = XPathResult.NUMBER_TYPE;
		} else if (v.constructor === XBoolean) {
			t = XPathResult.BOOLEAN_TYPE;
		} else if (v.constructor === XNodeSet) {
			t = XPathResult.UNORDERED_NODE_ITERATOR_TYPE;
		}
	}
	this.resultType = t;
	switch (t) {
		case XPathResult.NUMBER_TYPE:
			this.numberValue = v.numberValue();
			return;
		case XPathResult.STRING_TYPE:
			this.stringValue = v.stringValue();
			return;
		case XPathResult.BOOLEAN_TYPE:
			this.booleanValue = v.booleanValue();
			return;
		case XPathResult.ANY_UNORDERED_NODE_TYPE:
		case XPathResult.FIRST_ORDERED_NODE_TYPE:
			if (v.constructor === XNodeSet) {
				this.singleNodeValue = v.first();
				return;
			}
			break;
		case XPathResult.UNORDERED_NODE_ITERATOR_TYPE:
		case XPathResult.ORDERED_NODE_ITERATOR_TYPE:
			if (v.constructor === XNodeSet) {
				this.invalidIteratorState = false;
				this.nodes = v.toArray();
				this.iteratorIndex = 0;
				return;
			}
			break;
		case XPathResult.UNORDERED_NODE_SNAPSHOT_TYPE:
		case XPathResult.ORDERED_NODE_SNAPSHOT_TYPE:
			if (v.constructor === XNodeSet) {
				this.nodes = v.toArray();
				this.snapshotLength = this.nodes.length;
				return;
			}
			break;
	}
	throw new XPathException(XPathException.TYPE_ERR);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString"></a>[function <span class="apidocSignatureSpan">xpath.</span>XString (s)](#apidoc.element.xpath.XString)
- description and source-code
```javascript
function XString(s) {
	if (arguments.length > 0) {
		this.init(s);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.createExpression"></a>[function <span class="apidocSignatureSpan">xpath.</span>createExpression (e, r)](#apidoc.element.xpath.createExpression)
- description and source-code
```javascript
createExpression = function (e, r) {
		try {
			return new XPathExpression(e, r, p);
		} catch (e) {
			throw new XPathException(XPathException.INVALID_EXPRESSION_ERR, e);
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.createNSResolver"></a>[function <span class="apidocSignatureSpan">xpath.</span>createNSResolver (n)](#apidoc.element.xpath.createNSResolver)
- description and source-code
```javascript
createNSResolver = function (n) {
		return new NodeXPathNSResolver(n);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.evaluate"></a>[function <span class="apidocSignatureSpan">xpath.</span>evaluate (e, cn, r, t, res)](#apidoc.element.xpath.evaluate)
- description and source-code
```javascript
evaluate = function (e, cn, r, t, res) {
		if (t < 0 || t > 9) {
			throw { code: 0, toString: function() { return "Request type not supported"; } };
		}
        return doc.createExpression(e, r, p).evaluate(cn, t, res);
	}
```
- example usage
```shell
...

Using the same interface you have on modern browsers ([MDN])

'''''javascript
var node = null;
var xml = "<book author='J. K. Rowling'><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var result = xpath.evaluate(
    "/book/title",            // xpathExpression
    doc,                        // contextNode
    null,                       // namespaceResolver
    xpath.XPathResult.ANY_TYPE, // resultType
    null                        // result
)
...
```

#### <a name="apidoc.element.xpath.parse"></a>[function <span class="apidocSignatureSpan">xpath.</span>parse (xpath)](#apidoc.element.xpath.parse)
- description and source-code
```javascript
function parse(xpath) {
    var parsed = parser.parse(xpath);

    return Object.create(evaluatorPrototype, {
        expression: {
            value: parsed
        }
    });
}
```
- example usage
```shell
...
		assert.ok(Number.isNaN(xpath.select('number("2e9")')), 'number("2e9")');
		assert.ok(Number.isNaN(xpath.select('number("+33")')), 'number("+33")');
		
		test.done();
	}
	
	,'correct number to string conversion': function (test) {
		assert.equal('0.0000000000000000000000005250000000000001', xpath.parse('0.525 div 1000000 div 1000000 div 1000000 div 1000000').
evaluateString());
		assert.equal('525000000000000000000000', xpath.parse('0.525 * 1000000 * 1000000 * 1000000 * 1000000').evaluateString());
		
		test.done();
	}
	
	,'local-name() and name() of processing instruction': function (test) {
	    var xml = '<?book-record added="2015-01-16" author="J.K. Rowling" ?><book>Harry Potter</book>';
...
```

#### <a name="apidoc.element.xpath.select"></a>[function <span class="apidocSignatureSpan">xpath.</span>select (e, doc, single)](#apidoc.element.xpath.select)
- description and source-code
```javascript
select = function (e, doc, single) {
	return exports.selectWithResolver(e, doc, null, single);
}
```
- example usage
```shell
...
## Your first xpath:
'''''javascript
var xpath = require('xpath')
  , dom = require('xmldom').DOMParser

var xml = "<book><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var nodes = xpath.select("//title", doc)

console.log(nodes[0].localName + ": " + nodes[0].firstChild.data)
console.log("Node: " + nodes[0].toString())
'''''
➡

title: Harry Potter
...
```

#### <a name="apidoc.element.xpath.select1"></a>[function <span class="apidocSignatureSpan">xpath.</span>select1 (e, doc)](#apidoc.element.xpath.select1)
- description and source-code
```javascript
select1 = function (e, doc) {
	return exports.select(e, doc, true);
}
```
- example usage
```shell
...

Harry Potter

## Attributes
'''''javascript
var xml = "<book author='J. K. Rowling'><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var author = xpath.select1("/book/@author", doc).value

console.log(author)
'''''
➡

J. K. Rowling
...
```

#### <a name="apidoc.element.xpath.selectWithResolver"></a>[function <span class="apidocSignatureSpan">xpath.</span>selectWithResolver (e, doc, resolver, single)](#apidoc.element.xpath.selectWithResolver)
- description and source-code
```javascript
selectWithResolver = function (e, doc, resolver, single) {
	var expression = new XPathExpression(e, resolver, new XPathParser());
	var type = XPathResult.ANY_TYPE;

	var result = expression.evaluate(doc, type, null);

	if (result.resultType == XPathResult.STRING_TYPE) {
		result = result.stringValue;
	}
	else if (result.resultType == XPathResult.NUMBER_TYPE) {
		result = result.numberValue;
	}
	else if (result.resultType == XPathResult.BOOLEAN_TYPE) {
		result = result.booleanValue;
	}
	else {
		result = result.nodes;
		if (single) {
			result = result[0];
		}
	}

	return result;
}
```
- example usage
```shell
...
				'testns': 'http://example.com/test'
			},
			lookupNamespaceURI: function(prefix) {
				return this.mappings[prefix];
			}
		}

		var nodes = xpath.selectWithResolver('//testns:title/text()', doc, resolver);
		assert.equal('Harry Potter', xpath.selectWithResolver('//testns:title/text()', doc, resolver)[0].nodeValue);
		assert.equal('JKR', xpath.selectWithResolver('//testns:field[@testns:type="author"]/text()', doc, resolver)[0].nodeValue);

		test.done();
	},

	'select xpath with default namespace, using a resolver': function (test) {
...
```

#### <a name="apidoc.element.xpath.useNamespaces"></a>[function <span class="apidocSignatureSpan">xpath.</span>useNamespaces (mappings)](#apidoc.element.xpath.useNamespaces)
- description and source-code
```javascript
useNamespaces = function (mappings) {
	var resolver = {
		mappings: mappings || {},
		lookupNamespaceURI: function(prefix) {
			return this.mappings[prefix];
		}
	};

	return function(e, doc, single) {
		return exports.selectWithResolver(e, doc, resolver, single);
	};
}
```
- example usage
```shell
...
➡

myns

## Namespaces with easy mappings
'''''javascript
var xml = "<book xmlns:bookml='http://example.com/book'><bookml:title>Harry Potter</bookml:title></book>"
var select = xpath.useNamespaces({"bookml": "http://example.com/book"});

console.log(select('//bookml:title/text()', doc)[0].nodeValue);
'''''
➡

Harry Potter
...
```



# <a name="apidoc.module.xpath.BarOperation"></a>[module xpath.BarOperation](#apidoc.module.xpath.BarOperation)

#### <a name="apidoc.element.xpath.BarOperation.BarOperation"></a>[function <span class="apidocSignatureSpan">xpath.</span>BarOperation (lhs, rhs)](#apidoc.element.xpath.BarOperation.BarOperation)
- description and source-code
```javascript
function BarOperation(lhs, rhs) {
	if (arguments.length > 0) {
		this.init(lhs, rhs);
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.BarOperation.prototype"></a>[module xpath.BarOperation.prototype](#apidoc.module.xpath.BarOperation.prototype)

#### <a name="apidoc.element.xpath.BarOperation.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.BarOperation.prototype.</span>constructor (lhs, rhs)](#apidoc.element.xpath.BarOperation.prototype.constructor)
- description and source-code
```javascript
function BarOperation(lhs, rhs) {
	if (arguments.length > 0) {
		this.init(lhs, rhs);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.BarOperation.prototype.evaluate"></a>[function <span class="apidocSignatureSpan">xpath.BarOperation.prototype.</span>evaluate (c)](#apidoc.element.xpath.BarOperation.prototype.evaluate)
- description and source-code
```javascript
evaluate = function (c) {
	return this.lhs.evaluate(c).nodeset().union(this.rhs.evaluate(c).nodeset());
}
```
- example usage
```shell
...

Using the same interface you have on modern browsers ([MDN])

'''''javascript
var node = null;
var xml = "<book author='J. K. Rowling'><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var result = xpath.evaluate(
    "/book/title",            // xpathExpression
    doc,                        // contextNode
    null,                       // namespaceResolver
    xpath.XPathResult.ANY_TYPE, // resultType
    null                        // result
)
...
```

#### <a name="apidoc.element.xpath.BarOperation.prototype.init"></a>[function <span class="apidocSignatureSpan">xpath.BarOperation.prototype.</span>init (lhs, rhs)](#apidoc.element.xpath.BarOperation.prototype.init)
- description and source-code
```javascript
init = function (lhs, rhs) {
	BarOperation.superclass.init.call(this, lhs, rhs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.BarOperation.prototype.toString"></a>[function <span class="apidocSignatureSpan">xpath.BarOperation.prototype.</span>toString ()](#apidoc.element.xpath.BarOperation.prototype.toString)
- description and source-code
```javascript
toString = function () {
	return this.lhs.toString() + " | " + this.rhs.toString();
}
```
- example usage
```shell
...
  , dom = require('xmldom').DOMParser

var xml = "<book><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var nodes = xpath.select("//title", doc)

console.log(nodes[0].localName + ": " + nodes[0].firstChild.data)
console.log("Node: " + nodes[0].toString())
'''''
➡

    title: Harry Potter
    Node: <title>Harry Potter</title>

### Alternatively
...
```



# <a name="apidoc.module.xpath.BarOperation.superclass"></a>[module xpath.BarOperation.superclass](#apidoc.module.xpath.BarOperation.superclass)

#### <a name="apidoc.element.xpath.BarOperation.superclass.constructor"></a>[function <span class="apidocSignatureSpan">xpath.BarOperation.superclass.</span>constructor (lhs, rhs)](#apidoc.element.xpath.BarOperation.superclass.constructor)
- description and source-code
```javascript
function BinaryOperation(lhs, rhs) {
	if (arguments.length > 0) {
		this.init(lhs, rhs);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.BarOperation.superclass.init"></a>[function <span class="apidocSignatureSpan">xpath.BarOperation.superclass.</span>init (lhs, rhs)](#apidoc.element.xpath.BarOperation.superclass.init)
- description and source-code
```javascript
init = function (lhs, rhs) {
	this.lhs = lhs;
	this.rhs = rhs;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.FunctionResolver"></a>[module xpath.FunctionResolver](#apidoc.module.xpath.FunctionResolver)

#### <a name="apidoc.element.xpath.FunctionResolver.FunctionResolver"></a>[function <span class="apidocSignatureSpan">xpath.</span>FunctionResolver (thisArg)](#apidoc.element.xpath.FunctionResolver.FunctionResolver)
- description and source-code
```javascript
function FunctionResolver(thisArg) {
	this.thisArg = thisArg != null ? thisArg : Functions;
	this.functions = new Object();
	this.addStandardFunctions();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.FunctionResolver.getFunctionFromContext"></a>[function <span class="apidocSignatureSpan">xpath.FunctionResolver.</span>getFunctionFromContext (qName, context)](#apidoc.element.xpath.FunctionResolver.getFunctionFromContext)
- description and source-code
```javascript
getFunctionFromContext = function (qName, context) {
    var parts = Utilities.resolveQName(qName, context.namespaceResolver, context.contextNode, false);

    if (parts[0] === null) {
        throw new Error("Cannot resolve QName " + name);
    }

    return context.functionResolver.getFunction(parts[1], parts[0]);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.FunctionResolver.prototype"></a>[module xpath.FunctionResolver.prototype](#apidoc.module.xpath.FunctionResolver.prototype)

#### <a name="apidoc.element.xpath.FunctionResolver.prototype.addFunction"></a>[function <span class="apidocSignatureSpan">xpath.FunctionResolver.prototype.</span>addFunction (ns, ln, f)](#apidoc.element.xpath.FunctionResolver.prototype.addFunction)
- description and source-code
```javascript
addFunction = function (ns, ln, f) {
	this.functions["{" + ns + "}" + ln] = f;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.FunctionResolver.prototype.addStandardFunctions"></a>[function <span class="apidocSignatureSpan">xpath.FunctionResolver.prototype.</span>addStandardFunctions ()](#apidoc.element.xpath.FunctionResolver.prototype.addStandardFunctions)
- description and source-code
```javascript
addStandardFunctions = function () {
	this.functions["{}last"] = Functions.last;
	this.functions["{}position"] = Functions.position;
	this.functions["{}count"] = Functions.count;
	this.functions["{}id"] = Functions.id;
	this.functions["{}local-name"] = Functions.localName;
	this.functions["{}namespace-uri"] = Functions.namespaceURI;
	this.functions["{}name"] = Functions.name;
	this.functions["{}string"] = Functions.string;
	this.functions["{}concat"] = Functions.concat;
	this.functions["{}starts-with"] = Functions.startsWith;
	this.functions["{}contains"] = Functions.contains;
	this.functions["{}substring-before"] = Functions.substringBefore;
	this.functions["{}substring-after"] = Functions.substringAfter;
	this.functions["{}substring"] = Functions.substring;
	this.functions["{}string-length"] = Functions.stringLength;
	this.functions["{}normalize-space"] = Functions.normalizeSpace;
	this.functions["{}translate"] = Functions.translate;
	this.functions["{}boolean"] = Functions.boolean_;
	this.functions["{}not"] = Functions.not;
	this.functions["{}true"] = Functions.true_;
	this.functions["{}false"] = Functions.false_;
	this.functions["{}lang"] = Functions.lang;
	this.functions["{}number"] = Functions.number;
	this.functions["{}sum"] = Functions.sum;
	this.functions["{}floor"] = Functions.floor;
	this.functions["{}ceiling"] = Functions.ceiling;
	this.functions["{}round"] = Functions.round;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.FunctionResolver.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.FunctionResolver.prototype.</span>constructor (thisArg)](#apidoc.element.xpath.FunctionResolver.prototype.constructor)
- description and source-code
```javascript
function FunctionResolver(thisArg) {
	this.thisArg = thisArg != null ? thisArg : Functions;
	this.functions = new Object();
	this.addStandardFunctions();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.FunctionResolver.prototype.getFunction"></a>[function <span class="apidocSignatureSpan">xpath.FunctionResolver.prototype.</span>getFunction (localName, namespace)](#apidoc.element.xpath.FunctionResolver.prototype.getFunction)
- description and source-code
```javascript
getFunction = function (localName, namespace) {
	return this.functions["{" + namespace + "}" + localName];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.NamespaceResolver"></a>[module xpath.NamespaceResolver](#apidoc.module.xpath.NamespaceResolver)

#### <a name="apidoc.element.xpath.NamespaceResolver.NamespaceResolver"></a>[function <span class="apidocSignatureSpan">xpath.</span>NamespaceResolver ()](#apidoc.element.xpath.NamespaceResolver.NamespaceResolver)
- description and source-code
```javascript
function NamespaceResolver() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.NamespaceResolver.prototype"></a>[module xpath.NamespaceResolver.prototype](#apidoc.module.xpath.NamespaceResolver.prototype)

#### <a name="apidoc.element.xpath.NamespaceResolver.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.NamespaceResolver.prototype.</span>constructor ()](#apidoc.element.xpath.NamespaceResolver.prototype.constructor)
- description and source-code
```javascript
function NamespaceResolver() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.NamespaceResolver.prototype.getNamespace"></a>[function <span class="apidocSignatureSpan">xpath.NamespaceResolver.prototype.</span>getNamespace (prefix, n)](#apidoc.element.xpath.NamespaceResolver.prototype.getNamespace)
- description and source-code
```javascript
getNamespace = function (prefix, n) {
	if (prefix == "xml") {
		return XPath.XML_NAMESPACE_URI;
	} else if (prefix == "xmlns") {
		return XPath.XMLNS_NAMESPACE_URI;
	}
	if (n.nodeType == 9 /*Node.DOCUMENT_NODE*/) {
		n = n.documentElement;
	} else if (n.nodeType == 2 /*Node.ATTRIBUTE_NODE*/) {
		n = PathExpr.prototype.getOwnerElement(n);
	} else if (n.nodeType != 1 /*Node.ELEMENT_NODE*/) {
		n = n.parentNode;
	}
	while (n != null && n.nodeType == 1 /*Node.ELEMENT_NODE*/) {
		var nnm = n.attributes;
		for (var i = 0; i < nnm.length; i++) {
			var a = nnm.item(i);
			var aname = a.name || a.nodeName;
			if ((aname === "xmlns" && prefix === "")
					|| aname === "xmlns:" + prefix) {
				return String(a.value || a.nodeValue);
			}
		}
		n = n.parentNode;
	}
	return null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.NodeTest"></a>[module xpath.NodeTest](#apidoc.module.xpath.NodeTest)

#### <a name="apidoc.element.xpath.NodeTest.NodeTest"></a>[function <span class="apidocSignatureSpan">xpath.</span>NodeTest (type, value)](#apidoc.element.xpath.NodeTest.NodeTest)
- description and source-code
```javascript
function NodeTest(type, value) {
	if (arguments.length > 0) {
		this.init(type, value);
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.NodeTest.prototype"></a>[module xpath.NodeTest.prototype](#apidoc.module.xpath.NodeTest.prototype)

#### <a name="apidoc.element.xpath.NodeTest.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.NodeTest.prototype.</span>constructor (type, value)](#apidoc.element.xpath.NodeTest.prototype.constructor)
- description and source-code
```javascript
function NodeTest(type, value) {
	if (arguments.length > 0) {
		this.init(type, value);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.NodeTest.prototype.init"></a>[function <span class="apidocSignatureSpan">xpath.NodeTest.prototype.</span>init (type, value)](#apidoc.element.xpath.NodeTest.prototype.init)
- description and source-code
```javascript
init = function (type, value) {
	this.type = type;
	this.value = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.NodeTest.prototype.matches"></a>[function <span class="apidocSignatureSpan">xpath.NodeTest.prototype.</span>matches (n, xpc)](#apidoc.element.xpath.NodeTest.prototype.matches)
- description and source-code
```javascript
matches = function (n, xpc) {
    var nType = n.nodeType;

	switch (this.type) {
		case NodeTest.NAMETESTANY:
			if (nType === 2 /*Node.ATTRIBUTE_NODE*/
					|| nType === 1 /*Node.ELEMENT_NODE*/
					|| nType === XPathNamespace.XPATH_NAMESPACE_NODE) {
				return true;
			}
			return false;
		case NodeTest.NAMETESTPREFIXANY:
			if (nType === 2 /*Node.ATTRIBUTE_NODE*/ || nType === 1 /*Node.ELEMENT_NODE*/) {
				var ns = xpc.namespaceResolver.getNamespace(this.value, xpc.expressionContextNode);
				if (ns == null) {
					throw new Error("Cannot resolve QName " + this.value);
				}
				return ns === (n.namespaceURI || '');
			}
			return false;
		case NodeTest.NAMETESTQNAME:
			if (nType === 2 /*Node.ATTRIBUTE_NODE*/
					|| nType === 1 /*Node.ELEMENT_NODE*/
					|| nType === XPathNamespace.XPATH_NAMESPACE_NODE) {
				var test = Utilities.resolveQName(this.value, xpc.namespaceResolver, xpc.expressionContextNode, false);
				if (test[0] == null) {
					throw new Error("Cannot resolve QName " + this.value);
				}

				test[0] = String(test[0]) || null;
				test[1] = String(test[1]);

				var node = [
                    String(n.namespaceURI || '') || null,
                    // localName will be null if the node was created with DOM1 createElement()
                    String(n.localName || n.nodeName)
                ];

				if (xpc.caseInsensitive) {
					return test[0] === node[0] && test[1].toLowerCase() === node[1].toLowerCase();
				}

				return test[0] === node[0] && test[1] === node[1];
			}
			return false;
		case NodeTest.COMMENT:
			return nType === 8 /*Node.COMMENT_NODE*/;
		case NodeTest.TEXT:
			return nType === 3 /*Node.TEXT_NODE*/ || nType == 4 /*Node.CDATA_SECTION_NODE*/;
		case NodeTest.PI:
			return nType === 7 /*Node.PROCESSING_INSTRUCTION_NODE*/
				&& (this.value == null || n.nodeName == this.value);
		case NodeTest.NODE:
			return nType === 9 /*Node.DOCUMENT_NODE*/
				|| nType === 1 /*Node.ELEMENT_NODE*/
				|| nType === 2 /*Node.ATTRIBUTE_NODE*/
				|| nType === 3 /*Node.TEXT_NODE*/
				|| nType === 4 /*Node.CDATA_SECTION_NODE*/
				|| nType === 8 /*Node.COMMENT_NODE*/
				|| nType === 7 /*Node.PROCESSING_INSTRUCTION_NODE*/;
	}
	return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.NodeTest.prototype.toString"></a>[function <span class="apidocSignatureSpan">xpath.NodeTest.prototype.</span>toString ()](#apidoc.element.xpath.NodeTest.prototype.toString)
- description and source-code
```javascript
toString = function () {
	switch (this.type) {
		case NodeTest.NAMETESTANY:
			return "*";
		case NodeTest.NAMETESTPREFIXANY:
			return this.value + ":*";
		case NodeTest.NAMETESTRESOLVEDANY:
			return "{" + this.value + "}*";
		case NodeTest.NAMETESTQNAME:
			return this.value;
		case NodeTest.NAMETESTRESOLVEDNAME:
			return "{" + this.namespaceURI + "}" + this.value;
		case NodeTest.COMMENT:
			return "comment()";
		case NodeTest.TEXT:
			return "text()";
		case NodeTest.PI:
			if (this.value != undefined) {
				return "processing-instruction(\"" + this.value + "\")";
			}
			return "processing-instruction()";
		case NodeTest.NODE:
			return "node()";
	}
	return "<unknown nodetest type>";
}
```
- example usage
```shell
...
  , dom = require('xmldom').DOMParser

var xml = "<book><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var nodes = xpath.select("//title", doc)

console.log(nodes[0].localName + ": " + nodes[0].firstChild.data)
console.log("Node: " + nodes[0].toString())
'''''
➡

    title: Harry Potter
    Node: <title>Harry Potter</title>

### Alternatively
...
```



# <a name="apidoc.module.xpath.Step"></a>[module xpath.Step](#apidoc.module.xpath.Step)

#### <a name="apidoc.element.xpath.Step.Step"></a>[function <span class="apidocSignatureSpan">xpath.</span>Step (axis, nodetest, preds)](#apidoc.element.xpath.Step.Step)
- description and source-code
```javascript
function Step(axis, nodetest, preds) {
	if (arguments.length > 0) {
		this.init(axis, nodetest, preds);
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.Step.prototype"></a>[module xpath.Step.prototype](#apidoc.module.xpath.Step.prototype)

#### <a name="apidoc.element.xpath.Step.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.Step.prototype.</span>constructor (axis, nodetest, preds)](#apidoc.element.xpath.Step.prototype.constructor)
- description and source-code
```javascript
function Step(axis, nodetest, preds) {
	if (arguments.length > 0) {
		this.init(axis, nodetest, preds);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.Step.prototype.init"></a>[function <span class="apidocSignatureSpan">xpath.Step.prototype.</span>init (axis, nodetest, preds)](#apidoc.element.xpath.Step.prototype.init)
- description and source-code
```javascript
init = function (axis, nodetest, preds) {
	this.axis = axis;
	this.nodeTest = nodetest;
	this.predicates = preds;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.Step.prototype.toString"></a>[function <span class="apidocSignatureSpan">xpath.Step.prototype.</span>toString ()](#apidoc.element.xpath.Step.prototype.toString)
- description and source-code
```javascript
toString = function () {
	var s;
	switch (this.axis) {
		case Step.ANCESTOR:
			s = "ancestor";
			break;
		case Step.ANCESTORORSELF:
			s = "ancestor-or-self";
			break;
		case Step.ATTRIBUTE:
			s = "attribute";
			break;
		case Step.CHILD:
			s = "child";
			break;
		case Step.DESCENDANT:
			s = "descendant";
			break;
		case Step.DESCENDANTORSELF:
			s = "descendant-or-self";
			break;
		case Step.FOLLOWING:
			s = "following";
			break;
		case Step.FOLLOWINGSIBLING:
			s = "following-sibling";
			break;
		case Step.NAMESPACE:
			s = "namespace";
			break;
		case Step.PARENT:
			s = "parent";
			break;
		case Step.PRECEDING:
			s = "preceding";
			break;
		case Step.PRECEDINGSIBLING:
			s = "preceding-sibling";
			break;
		case Step.SELF:
			s = "self";
			break;
	}
	s += "::";
	s += this.nodeTest.toString();
	for (var i = 0; i < this.predicates.length; i++) {
		s += "[" + this.predicates[i].toString() + "]";
	}
	return s;
}
```
- example usage
```shell
...
  , dom = require('xmldom').DOMParser

var xml = "<book><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var nodes = xpath.select("//title", doc)

console.log(nodes[0].localName + ": " + nodes[0].firstChild.data)
console.log("Node: " + nodes[0].toString())
'''''
➡

    title: Harry Potter
    Node: <title>Harry Potter</title>

### Alternatively
...
```



# <a name="apidoc.module.xpath.Utilities"></a>[module xpath.Utilities](#apidoc.module.xpath.Utilities)

#### <a name="apidoc.element.xpath.Utilities.coalesceText"></a>[function <span class="apidocSignatureSpan">xpath.Utilities.</span>coalesceText (n)](#apidoc.element.xpath.Utilities.coalesceText)
- description and source-code
```javascript
coalesceText = function (n) {
	for (var m = n.firstChild; m != null; m = m.nextSibling) {
		if (m.nodeType == 3 /*Node.TEXT_NODE*/ || m.nodeType == 4 /*Node.CDATA_SECTION_NODE*/) {
			var s = m.nodeValue;
			var first = m;
			m = m.nextSibling;
			while (m != null && (m.nodeType == 3 /*Node.TEXT_NODE*/ || m.nodeType == 4 /*Node.CDATA_SECTION_NODE*/)) {
				s += m.nodeValue;
				var del = m;
				m = m.nextSibling;
				del.parentNode.removeChild(del);
			}
			if (first.nodeType == 4 /*Node.CDATA_SECTION_NODE*/) {
				var p = first.parentNode;
				if (first.nextSibling == null) {
					p.removeChild(first);
					p.appendChild(p.ownerDocument.createTextNode(s));
				} else {
					var next = first.nextSibling;
					p.removeChild(first);
					p.insertBefore(p.ownerDocument.createTextNode(s), next);
				}
			} else {
				first.nodeValue = s;
			}
			if (m == null) {
				break;
			}
		} else if (m.nodeType == 1 /*Node.ELEMENT_NODE*/) {
			Utilities.coalesceText(m);
		}
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.Utilities.getElementById"></a>[function <span class="apidocSignatureSpan">xpath.Utilities.</span>getElementById (n, id)](#apidoc.element.xpath.Utilities.getElementById)
- description and source-code
```javascript
getElementById = function (n, id) {
	// Note that this does not check the DTD to check for actual
	// attributes of type ID, so this may be a bit wrong.
	if (n.nodeType == 1 /*Node.ELEMENT_NODE*/) {
		if (n.getAttribute("id") == id
				|| n.getAttributeNS(null, "id") == id) {
			return n;
		}
	}
	for (var m = n.firstChild; m != null; m = m.nextSibling) {
		var res = Utilities.getElementById(m, id);
		if (res != null) {
			return res;
		}
	}
	return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.Utilities.instance_of"></a>[function <span class="apidocSignatureSpan">xpath.Utilities.</span>instance_of (o, c)](#apidoc.element.xpath.Utilities.instance_of)
- description and source-code
```javascript
instance_of = function (o, c) {
	while (o != null) {
		if (o.constructor === c) {
			return true;
		}
		if (o === Object) {
			return false;
		}
		o = o.constructor.superclass;
	}
	return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.Utilities.isAttribute"></a>[function <span class="apidocSignatureSpan">xpath.Utilities.</span>isAttribute (val)](#apidoc.element.xpath.Utilities.isAttribute)
- description and source-code
```javascript
isAttribute = function (val) {
    return val && (val.nodeType === 2 || val.ownerElement);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.Utilities.isLetter"></a>[function <span class="apidocSignatureSpan">xpath.Utilities.</span>isLetter (c)](#apidoc.element.xpath.Utilities.isLetter)
- description and source-code
```javascript
isLetter = function (c) {
	return c >= 0x0041 && c <= 0x005A ||
		c >= 0x0061 && c <= 0x007A ||
		c >= 0x00C0 && c <= 0x00D6 ||
		c >= 0x00D8 && c <= 0x00F6 ||
		c >= 0x00F8 && c <= 0x00FF ||
		c >= 0x0100 && c <= 0x0131 ||
		c >= 0x0134 && c <= 0x013E ||
		c >= 0x0141 && c <= 0x0148 ||
		c >= 0x014A && c <= 0x017E ||
		c >= 0x0180 && c <= 0x01C3 ||
		c >= 0x01CD && c <= 0x01F0 ||
		c >= 0x01F4 && c <= 0x01F5 ||
		c >= 0x01FA && c <= 0x0217 ||
		c >= 0x0250 && c <= 0x02A8 ||
		c >= 0x02BB && c <= 0x02C1 ||
		c == 0x0386 ||
		c >= 0x0388 && c <= 0x038A ||
		c == 0x038C ||
		c >= 0x038E && c <= 0x03A1 ||
		c >= 0x03A3 && c <= 0x03CE ||
		c >= 0x03D0 && c <= 0x03D6 ||
		c == 0x03DA ||
		c == 0x03DC ||
		c == 0x03DE ||
		c == 0x03E0 ||
		c >= 0x03E2 && c <= 0x03F3 ||
		c >= 0x0401 && c <= 0x040C ||
		c >= 0x040E && c <= 0x044F ||
		c >= 0x0451 && c <= 0x045C ||
		c >= 0x045E && c <= 0x0481 ||
		c >= 0x0490 && c <= 0x04C4 ||
		c >= 0x04C7 && c <= 0x04C8 ||
		c >= 0x04CB && c <= 0x04CC ||
		c >= 0x04D0 && c <= 0x04EB ||
		c >= 0x04EE && c <= 0x04F5 ||
		c >= 0x04F8 && c <= 0x04F9 ||
		c >= 0x0531 && c <= 0x0556 ||
		c == 0x0559 ||
		c >= 0x0561 && c <= 0x0586 ||
		c >= 0x05D0 && c <= 0x05EA ||
		c >= 0x05F0 && c <= 0x05F2 ||
		c >= 0x0621 && c <= 0x063A ||
		c >= 0x0641 && c <= 0x064A ||
		c >= 0x0671 && c <= 0x06B7 ||
		c >= 0x06BA && c <= 0x06BE ||
		c >= 0x06C0 && c <= 0x06CE ||
		c >= 0x06D0 && c <= 0x06D3 ||
		c == 0x06D5 ||
		c >= 0x06E5 && c <= 0x06E6 ||
		c >= 0x0905 && c <= 0x0939 ||
		c == 0x093D ||
		c >= 0x0958 && c <= 0x0961 ||
		c >= 0x0985 && c <= 0x098C ||
		c >= 0x098F && c <= 0x0990 ||
		c >= 0x0993 && c <= 0x09A8 ||
		c >= 0x09AA && c <= 0x09B0 ||
		c == 0x09B2 ||
		c >= 0x09B6 && c <= 0x09B9 ||
		c >= 0x09DC && c <= 0x09DD ||
		c >= 0x09DF && c <= 0x09E1 ||
		c >= 0x09F0 && c <= 0x09F1 ||
		c >= 0x0A05 && c <= 0x0A0A ||
		c >= 0x0A0F && c <= 0x0A10 ||
		c >= 0x0A13 && c <= 0x0A28 ||
		c >= 0x0A2A && c <= 0x0A30 ||
		c >= 0x0A32 && c <= 0x0A33 ||
		c >= 0x0A35 && c <= 0x0A36 ||
		c >= 0x0A38 && c <= 0x0A39 ||
		c >= 0x0A59 && c <= 0x0A5C ||
		c == 0x0A5E ||
		c >= 0x0A72 && c <= 0x0A74 ||
		c >= 0x0A85 && c <= 0x0A8B ||
		c == 0x0A8D ||
		c >= 0x0A8F && c <= 0x0A91 ||
		c >= 0x0A93 && c <= 0x0AA8 ||
		c >= 0x0AAA && c <= 0x0AB0 ||
		c >= 0x0AB2 && c <= 0x0AB3 ||
		c >= 0x0AB5 && c <= 0x0AB9 ||
		c == 0x0ABD ||
		c == 0x0AE0 ||
		c >= 0x0B05 && c <= 0x0B0C ||
		c >= 0x0B0F && c <= 0x0B10 ||
		c >= 0x0B13 && c <= 0x0B28 ||
		c >= 0x0B2A && c <= 0x0B30 ||
		c >= 0x0B32 && c <= 0x0B33 ||
		c >= 0x0B36 && c <= 0x0B39 ||
		c == 0x0B3D ||
		c >= 0x0B5C && c <= 0x0B5D ||
		c >= 0x0B5F && c <= 0x0B61 ||
		c >= 0x0B85 && c <= 0x0B8A ||
		c >= 0x0B8E && c <= 0x0B90 ||
		c >= 0x0B92 && c <= 0x0B95 ||
		c >= 0x0B99 && c <= 0x0B9A ||
		c == 0x0B9C ||
		c >= 0x0B9E && c <= 0x0B9F ||
		c >= 0x0BA3 && c <= 0x0BA4 ||
		c >= 0x0BA8 && c <= 0x0BAA ||
		c >= 0x0BAE && c <= 0x0BB5 ||
		c >= 0x0BB7 && c <= 0x0BB9 ||
		c >= 0x0C05 && c <= 0x0C0C ||
		c >= 0x0C0E && c <= 0x0C10 ||
		c >= 0x0C12 && c <= 0x0C28 ||
		c >= 0x0C2A && c <= 0x0C33 ||
		c >= 0x0C35 && c <= 0x0C39 ||
		c >= 0x0C60 && c <= 0x0C61 ||
		c >= 0x0C85 && c <= 0x0C8C ||
		c >= 0x0C8E && c <= 0x0C90 ||
		c >= 0x0C92 && c <= 0x0CA8 ||
		c >= 0x0CAA && c <= 0x0CB3 ||
		c >= 0x0CB5 && c <= 0x0CB9 ||
		c == 0x0CDE ||
		c >= 0x0CE0 && c <= 0x0CE1 ||
		c >= 0x0D05 && c <= 0x0D0C ||
		c >= 0x0D0E && c <= 0x0D10 ||
		c >= 0x0D12 && c <= 0x0D28 ||
		c >= 0x0D2A && c <= 0x0D39 ||
		c >= 0x0D60 && c <= 0x0D61 ||
		c >= 0x0E01 && c <= 0x0E2E ||
		c == 0x0E30 ||
		c >= 0x0E32 && c <= 0x0E33 ||
		c >= 0x0E40 && c <= 0x0E45 ||
		c >= 0x0E81 && c <= 0x0E82 ||
		c == 0x0E84 ||
		c >= 0x0E87 && c <= 0x0E88 ||
		c == 0x0E8A ||
		c == 0x0E8D ||
		c >= 0x0E94 && c <= 0x0E97 ||
		c >= 0x0E99 && c <= 0x0E9F ||
		c >= 0x0EA1 && c <= 0x0EA3 ||
		c == 0x0EA5 ||
		c == 0x0EA7 ||
		c >= 0x0EAA && c <= 0x0EAB ||
		c >= 0x0EAD && c <= 0x0EAE ||
		c == 0x0EB0 ||
		c >= 0x0EB ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.Utilities.isNCNameChar"></a>[function <span class="apidocSignatureSpan">xpath.Utilities.</span>isNCNameChar (c)](#apidoc.element.xpath.Utilities.isNCNameChar)
- description and source-code
```javascript
isNCNameChar = function (c) {
	return c >= 0x0030 && c <= 0x0039
		|| c >= 0x0660 && c <= 0x0669
		|| c >= 0x06F0 && c <= 0x06F9
		|| c >= 0x0966 && c <= 0x096F
		|| c >= 0x09E6 && c <= 0x09EF
		|| c >= 0x0A66 && c <= 0x0A6F
		|| c >= 0x0AE6 && c <= 0x0AEF
		|| c >= 0x0B66 && c <= 0x0B6F
		|| c >= 0x0BE7 && c <= 0x0BEF
		|| c >= 0x0C66 && c <= 0x0C6F
		|| c >= 0x0CE6 && c <= 0x0CEF
		|| c >= 0x0D66 && c <= 0x0D6F
		|| c >= 0x0E50 && c <= 0x0E59
		|| c >= 0x0ED0 && c <= 0x0ED9
		|| c >= 0x0F20 && c <= 0x0F29
		|| c == 0x002E
		|| c == 0x002D
		|| c == 0x005F
		|| Utilities.isLetter(c)
		|| c >= 0x0300 && c <= 0x0345
		|| c >= 0x0360 && c <= 0x0361
		|| c >= 0x0483 && c <= 0x0486
		|| c >= 0x0591 && c <= 0x05A1
		|| c >= 0x05A3 && c <= 0x05B9
		|| c >= 0x05BB && c <= 0x05BD
		|| c == 0x05BF
		|| c >= 0x05C1 && c <= 0x05C2
		|| c == 0x05C4
		|| c >= 0x064B && c <= 0x0652
		|| c == 0x0670
		|| c >= 0x06D6 && c <= 0x06DC
		|| c >= 0x06DD && c <= 0x06DF
		|| c >= 0x06E0 && c <= 0x06E4
		|| c >= 0x06E7 && c <= 0x06E8
		|| c >= 0x06EA && c <= 0x06ED
		|| c >= 0x0901 && c <= 0x0903
		|| c == 0x093C
		|| c >= 0x093E && c <= 0x094C
		|| c == 0x094D
		|| c >= 0x0951 && c <= 0x0954
		|| c >= 0x0962 && c <= 0x0963
		|| c >= 0x0981 && c <= 0x0983
		|| c == 0x09BC
		|| c == 0x09BE
		|| c == 0x09BF
		|| c >= 0x09C0 && c <= 0x09C4
		|| c >= 0x09C7 && c <= 0x09C8
		|| c >= 0x09CB && c <= 0x09CD
		|| c == 0x09D7
		|| c >= 0x09E2 && c <= 0x09E3
		|| c == 0x0A02
		|| c == 0x0A3C
		|| c == 0x0A3E
		|| c == 0x0A3F
		|| c >= 0x0A40 && c <= 0x0A42
		|| c >= 0x0A47 && c <= 0x0A48
		|| c >= 0x0A4B && c <= 0x0A4D
		|| c >= 0x0A70 && c <= 0x0A71
		|| c >= 0x0A81 && c <= 0x0A83
		|| c == 0x0ABC
		|| c >= 0x0ABE && c <= 0x0AC5
		|| c >= 0x0AC7 && c <= 0x0AC9
		|| c >= 0x0ACB && c <= 0x0ACD
		|| c >= 0x0B01 && c <= 0x0B03
		|| c == 0x0B3C
		|| c >= 0x0B3E && c <= 0x0B43
		|| c >= 0x0B47 && c <= 0x0B48
		|| c >= 0x0B4B && c <= 0x0B4D
		|| c >= 0x0B56 && c <= 0x0B57
		|| c >= 0x0B82 && c <= 0x0B83
		|| c >= 0x0BBE && c <= 0x0BC2
		|| c >= 0x0BC6 && c <= 0x0BC8
		|| c >= 0x0BCA && c <= 0x0BCD
		|| c == 0x0BD7
		|| c >= 0x0C01 && c <= 0x0C03
		|| c >= 0x0C3E && c <= 0x0C44
		|| c >= 0x0C46 && c <= 0x0C48
		|| c >= 0x0C4A && c <= 0x0C4D
		|| c >= 0x0C55 && c <= 0x0C56
		|| c >= 0x0C82 && c <= 0x0C83
		|| c >= 0x0CBE && c <= 0x0CC4
		|| c >= 0x0CC6 && c <= 0x0CC8
		|| c >= 0x0CCA && c <= 0x0CCD
		|| c >= 0x0CD5 && c <= 0x0CD6
		|| c >= 0x0D02 && c <= 0x0D03
		|| c >= 0x0D3E && c <= 0x0D43
		|| c >= 0x0D46 && c <= 0x0D48
		|| c >= 0x0D4A && c <= 0x0D4D
		|| c == 0x0D57
		|| c == 0x0E31
		|| c >= 0x0E34 && c <= 0x0E3A
		|| c >= 0x0E47 && c <= 0x0E4E
		|| c == 0x0EB1
		|| c >= 0x0EB4 && c <= 0x0EB9
		|| c >= 0x0EBB && c <= 0x0EBC
		|| c >= 0x0EC8 && c <= 0x0ECD
		|| c >= 0x0F18 && c <= 0x0F19
		|| c == 0x0F35
		|| c == 0x0F37
		|| c == 0x0F39
		|| c == 0x0F3E
		|| c == 0x0F3F
		|| c >= 0x0F71 && c <= 0x0F84
		|| c >= 0x0F86 && c <= 0x0F8B
		|| c >= 0x0F90 && c <= 0x0F95
		|| c == 0x0F97
		|| c >= 0x0F99 && c <= 0x0FAD
		|| c >= 0x0FB1 && c <= 0x0FB7
		|| c == 0x0FB9
		|| c >= 0x20D0 && c <= 0x20DC
		|| c == 0x20E1
		|| c >= 0x302A && c <= 0x302F
		|| c == 0x3099
		|| c == 0x309A
		|| c == 0x00B7
		|| c == 0x02D0
		|| c == 0x02D1
		|| c == 0x0387
		|| c == 0x0640
		|| c == 0x0E46
		|| c == 0x0EC6
		|| c == 0x3005
		|| c >= 0x3031 && c <= 0x3035
		|| c >= 0x309D && c <= 0x309E
		|| c >= 0x30FC && c <= 0x30FE;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.Utilities.isSpace"></a>[function <span class="apidocSignatureSpan">xpath.Utilities.</span>isSpace (c)](#apidoc.element.xpath.Utilities.isSpace)
- description and source-code
```javascript
isSpace = function (c) {
	return c == 0x9 || c == 0xd || c == 0xa || c == 0x20;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.Utilities.resolveQName"></a>[function <span class="apidocSignatureSpan">xpath.Utilities.</span>resolveQName (qn, nr, n, useDefault)](#apidoc.element.xpath.Utilities.resolveQName)
- description and source-code
```javascript
resolveQName = function (qn, nr, n, useDefault) {
	var parts = Utilities.splitQName(qn);
	if (parts[0] != null) {
		parts[0] = nr.getNamespace(parts[0], n);
	} else {
		if (useDefault) {
			parts[0] = nr.getNamespace("", n);
			if (parts[0] == null) {
				parts[0] = "";
			}
		} else {
			parts[0] = "";
		}
	}
	return parts;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.Utilities.splitQName"></a>[function <span class="apidocSignatureSpan">xpath.Utilities.</span>splitQName (qn)](#apidoc.element.xpath.Utilities.splitQName)
- description and source-code
```javascript
splitQName = function (qn) {
	var i = qn.indexOf(":");
	if (i == -1) {
		return [ null, qn ];
	}
	return [ qn.substring(0, i), qn.substring(i + 1) ];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.VariableResolver"></a>[module xpath.VariableResolver](#apidoc.module.xpath.VariableResolver)

#### <a name="apidoc.element.xpath.VariableResolver.VariableResolver"></a>[function <span class="apidocSignatureSpan">xpath.</span>VariableResolver ()](#apidoc.element.xpath.VariableResolver.VariableResolver)
- description and source-code
```javascript
function VariableResolver() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.VariableResolver.prototype"></a>[module xpath.VariableResolver.prototype](#apidoc.module.xpath.VariableResolver.prototype)

#### <a name="apidoc.element.xpath.VariableResolver.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.VariableResolver.prototype.</span>constructor ()](#apidoc.element.xpath.VariableResolver.prototype.constructor)
- description and source-code
```javascript
function VariableResolver() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.VariableResolver.prototype.getVariable"></a>[function <span class="apidocSignatureSpan">xpath.VariableResolver.prototype.</span>getVariable (ln, ns)](#apidoc.element.xpath.VariableResolver.prototype.getVariable)
- description and source-code
```javascript
getVariable = function (ln, ns) {
	return null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XBoolean"></a>[module xpath.XBoolean](#apidoc.module.xpath.XBoolean)

#### <a name="apidoc.element.xpath.XBoolean.XBoolean"></a>[function <span class="apidocSignatureSpan">xpath.</span>XBoolean (b)](#apidoc.element.xpath.XBoolean.XBoolean)
- description and source-code
```javascript
function XBoolean(b) {
	if (arguments.length > 0) {
		this.init(b);
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XBoolean.prototype"></a>[module xpath.XBoolean.prototype](#apidoc.module.xpath.XBoolean.prototype)

#### <a name="apidoc.element.xpath.XBoolean.prototype.bool"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>bool ()](#apidoc.element.xpath.XBoolean.prototype.bool)
- description and source-code
```javascript
bool = function () {
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.booleanValue"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>booleanValue ()](#apidoc.element.xpath.XBoolean.prototype.booleanValue)
- description and source-code
```javascript
booleanValue = function () {
	return this.b;
}
```
- example usage
```shell
...
        var num = value.numberValue();
        return num * num;
    };

case "xor":
    return function (context, l, r) {
        assert.equal(3, arguments.length);
        var lbool = l.booleanValue();
        var rbool = r.booleanValue();
        return (lbool || rbool) && !(lbool && rbool);
    };

case "second":
    return function (context, nodes) {
        var nodesArr = nodes.toArray();
...
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>constructor (b)](#apidoc.element.xpath.XBoolean.prototype.constructor)
- description and source-code
```javascript
function XBoolean(b) {
	if (arguments.length > 0) {
		this.init(b);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.equals"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>equals (r)](#apidoc.element.xpath.XBoolean.prototype.equals)
- description and source-code
```javascript
equals = function (r) {
	if (Utilities.instance_of(r, XString) || Utilities.instance_of(r, XNumber)) {
		return this.equals(r.bool());
	}
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithBoolean(this, Operators.equals);
	}
	return new XBoolean(this.b == r.b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.evaluate"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>evaluate (c)](#apidoc.element.xpath.XBoolean.prototype.evaluate)
- description and source-code
```javascript
evaluate = function (c) {
	return this;
}
```
- example usage
```shell
...

Using the same interface you have on modern browsers ([MDN])

'''''javascript
var node = null;
var xml = "<book author='J. K. Rowling'><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var result = xpath.evaluate(
    "/book/title",            // xpathExpression
    doc,                        // contextNode
    null,                       // namespaceResolver
    xpath.XPathResult.ANY_TYPE, // resultType
    null                        // result
)
...
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.greaterthan"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>greaterthan (r)](#apidoc.element.xpath.XBoolean.prototype.greaterthan)
- description and source-code
```javascript
greaterthan = function (r) {
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this.number(), Operators.lessthanorequal);
	}
	return this.number().greaterthan(r.number());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.greaterthanorequal"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>greaterthanorequal (r)](#apidoc.element.xpath.XBoolean.prototype.greaterthanorequal)
- description and source-code
```javascript
greaterthanorequal = function (r) {
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this.number(), Operators.lessthan);
	}
	return this.number().greaterthanorequal(r.number());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.init"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>init (b)](#apidoc.element.xpath.XBoolean.prototype.init)
- description and source-code
```javascript
init = function (b) {
	this.b = Boolean(b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.lessthan"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>lessthan (r)](#apidoc.element.xpath.XBoolean.prototype.lessthan)
- description and source-code
```javascript
lessthan = function (r) {
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this.number(), Operators.greaterthanorequal);
	}
	return this.number().lessthan(r.number());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.lessthanorequal"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>lessthanorequal (r)](#apidoc.element.xpath.XBoolean.prototype.lessthanorequal)
- description and source-code
```javascript
lessthanorequal = function (r) {
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this.number(), Operators.greaterthan);
	}
	return this.number().lessthanorequal(r.number());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.nodeset"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>nodeset ()](#apidoc.element.xpath.XBoolean.prototype.nodeset)
- description and source-code
```javascript
nodeset = function () {
	throw new Error("Cannot convert boolean to nodeset");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.not"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>not ()](#apidoc.element.xpath.XBoolean.prototype.not)
- description and source-code
```javascript
not = function () {
	return new XBoolean(!this.b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.notequal"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>notequal (r)](#apidoc.element.xpath.XBoolean.prototype.notequal)
- description and source-code
```javascript
notequal = function (r) {
	if (Utilities.instance_of(r, XString) || Utilities.instance_of(r, XNumber)) {
		return this.notequal(r.bool());
	}
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithBoolean(this, Operators.notequal);
	}
	return new XBoolean(this.b != r.b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.number"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>number ()](#apidoc.element.xpath.XBoolean.prototype.number)
- description and source-code
```javascript
number = function () {
	return new XNumber(this.b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.numberValue"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>numberValue ()](#apidoc.element.xpath.XBoolean.prototype.numberValue)
- description and source-code
```javascript
numberValue = function () {
	return this.num().numberValue();
}
```
- example usage
```shell
...
    return function (context, value) {
        assert.equal(2, arguments.length);
        var str = value.stringValue();
        return str + str;
    };
case "square":
    return function (context, value) {
        var num = value.numberValue();
        return num * num;
    };

case "xor":
    return function (context, l, r) {
        assert.equal(3, arguments.length);
        var lbool = l.booleanValue();
...
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.string"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>string ()](#apidoc.element.xpath.XBoolean.prototype.string)
- description and source-code
```javascript
string = function () {
	return new XString(this.b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.stringValue"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>stringValue ()](#apidoc.element.xpath.XBoolean.prototype.stringValue)
- description and source-code
```javascript
stringValue = function () {
	return this.string().stringValue();
}
```
- example usage
```shell
...
		var xml = '<book><title>Harry Potter</title></book>';
var doc = new dom().parseFromString(xml);

var parsed = xpath.parse('concat(double(/*/title), " is cool")');

function doubleString(context, value) {
    assert.equal(2, arguments.length);
    var str = value.stringValue();
    return str + str;
}

function functions(name, namespace) {
    if(name === 'double') {
        return doubleString;
    }
...
```

#### <a name="apidoc.element.xpath.XBoolean.prototype.toString"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.prototype.</span>toString ()](#apidoc.element.xpath.XBoolean.prototype.toString)
- description and source-code
```javascript
toString = function () {
	return this.b.toString();
}
```
- example usage
```shell
...
  , dom = require('xmldom').DOMParser

var xml = "<book><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var nodes = xpath.select("//title", doc)

console.log(nodes[0].localName + ": " + nodes[0].firstChild.data)
console.log("Node: " + nodes[0].toString())
'''''
➡

    title: Harry Potter
    Node: <title>Harry Potter</title>

### Alternatively
...
```



# <a name="apidoc.module.xpath.XBoolean.superclass"></a>[module xpath.XBoolean.superclass](#apidoc.module.xpath.XBoolean.superclass)

#### <a name="apidoc.element.xpath.XBoolean.superclass.constructor"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.superclass.</span>constructor ()](#apidoc.element.xpath.XBoolean.superclass.constructor)
- description and source-code
```javascript
function Expression() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.superclass.evaluate"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.superclass.</span>evaluate (c)](#apidoc.element.xpath.XBoolean.superclass.evaluate)
- description and source-code
```javascript
evaluate = function (c) {
	throw new Error("Could not evaluate expression.");
}
```
- example usage
```shell
...

Using the same interface you have on modern browsers ([MDN])

'''''javascript
var node = null;
var xml = "<book author='J. K. Rowling'><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var result = xpath.evaluate(
    "/book/title",            // xpathExpression
    doc,                        // contextNode
    null,                       // namespaceResolver
    xpath.XPathResult.ANY_TYPE, // resultType
    null                        // result
)
...
```

#### <a name="apidoc.element.xpath.XBoolean.superclass.init"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.superclass.</span>init ()](#apidoc.element.xpath.XBoolean.superclass.init)
- description and source-code
```javascript
init = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XBoolean.superclass.toString"></a>[function <span class="apidocSignatureSpan">xpath.XBoolean.superclass.</span>toString ()](#apidoc.element.xpath.XBoolean.superclass.toString)
- description and source-code
```javascript
toString = function () {
	return "<Expression>";
}
```
- example usage
```shell
...
  , dom = require('xmldom').DOMParser

var xml = "<book><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var nodes = xpath.select("//title", doc)

console.log(nodes[0].localName + ": " + nodes[0].firstChild.data)
console.log("Node: " + nodes[0].toString())
'''''
➡

    title: Harry Potter
    Node: <title>Harry Potter</title>

### Alternatively
...
```



# <a name="apidoc.module.xpath.XNodeSet"></a>[module xpath.XNodeSet](#apidoc.module.xpath.XNodeSet)

#### <a name="apidoc.element.xpath.XNodeSet.XNodeSet"></a>[function <span class="apidocSignatureSpan">xpath.</span>XNodeSet ()](#apidoc.element.xpath.XNodeSet.XNodeSet)
- description and source-code
```javascript
function XNodeSet() {
	this.init();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XNodeSet.prototype"></a>[module xpath.XNodeSet.prototype](#apidoc.module.xpath.XNodeSet.prototype)

#### <a name="apidoc.element.xpath.XNodeSet.prototype.add"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>add (n)](#apidoc.element.xpath.XNodeSet.prototype.add)
- description and source-code
```javascript
add = function (n) {
    for (var i = 0; i < this.nodes.length; i += 1) {
        if (n === this.nodes[i]) {
            return;
        }
    }

    this.tree = null;
    this.nodes.push(n);
    this.size += 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.addArray"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>addArray (ns)](#apidoc.element.xpath.XNodeSet.prototype.addArray)
- description and source-code
```javascript
addArray = function (ns) {
	for (var i = 0; i < ns.length; i += 1) {
		this.add(ns[i]);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.bool"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>bool ()](#apidoc.element.xpath.XNodeSet.prototype.bool)
- description and source-code
```javascript
bool = function () {
	return new XBoolean(this.booleanValue());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.booleanValue"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>booleanValue ()](#apidoc.element.xpath.XNodeSet.prototype.booleanValue)
- description and source-code
```javascript
booleanValue = function () {
	return !!this.size;
}
```
- example usage
```shell
...
        var num = value.numberValue();
        return num * num;
    };

case "xor":
    return function (context, l, r) {
        assert.equal(3, arguments.length);
        var lbool = l.booleanValue();
        var rbool = r.booleanValue();
        return (lbool || rbool) && !(lbool && rbool);
    };

case "second":
    return function (context, nodes) {
        var nodesArr = nodes.toArray();
...
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.buildTree"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>buildTree ()](#apidoc.element.xpath.XNodeSet.prototype.buildTree)
- description and source-code
```javascript
buildTree = function () {
    if (!this.tree && this.nodes.length) {
        this.tree = new AVLTree(this.nodes[0]);
        for (var i = 1; i < this.nodes.length; i += 1) {
            this.tree.add(this.nodes[i]);
        }
    }

    return this.tree;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.compareWithBoolean"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>compareWithBoolean (r, o)](#apidoc.element.xpath.XNodeSet.prototype.compareWithBoolean)
- description and source-code
```javascript
compareWithBoolean = function (r, o) {
	return o(this.bool(), r);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.compareWithNodeSet"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>compareWithNodeSet (r, o)](#apidoc.element.xpath.XNodeSet.prototype.compareWithNodeSet)
- description and source-code
```javascript
compareWithNodeSet = function (r, o) {
	var arr = this.toUnsortedArray();
	var oInvert = function (lop, rop) { return o(rop, lop); };
	
	for (var i = 0; i < arr.length; i++) {
		var l = new XString(this.stringForNode(arr[i]));

		var res = r.compareWithString(l, oInvert);
		if (res.booleanValue()) {
			return res;
		}
	}
	
	return new XBoolean(false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.compareWithNumber"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>compareWithNumber (r, o)](#apidoc.element.xpath.XNodeSet.prototype.compareWithNumber)
- description and source-code
```javascript
compareWithNumber = function (r, o) {
	var a = this.toUnsortedArray();
	for (var i = 0; i < a.length; i++) {
		var n = a[i];
		var l = new XNumber(this.stringForNode(n));
		var res = o(l, r);
		if (res.booleanValue()) {
			return res;
		}
	}
	return new XBoolean(false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.compareWithString"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>compareWithString (r, o)](#apidoc.element.xpath.XNodeSet.prototype.compareWithString)
- description and source-code
```javascript
compareWithString = function (r, o) {
	var a = this.toUnsortedArray();
	for (var i = 0; i < a.length; i++) {
		var n = a[i];
		var l = new XString(this.stringForNode(n));
		var res = o(l, r);
		if (res.booleanValue()) {
			return res;
		}
	}
	return new XBoolean(false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>constructor ()](#apidoc.element.xpath.XNodeSet.prototype.constructor)
- description and source-code
```javascript
function XNodeSet() {
	this.init();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.equals"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>equals (r)](#apidoc.element.xpath.XNodeSet.prototype.equals)
- description and source-code
```javascript
equals = function (r) {
	if (Utilities.instance_of(r, XString)) {
		return this.compareWithString(r, Operators.equals);
	}
	if (Utilities.instance_of(r, XNumber)) {
		return this.compareWithNumber(r, Operators.equals);
	}
	if (Utilities.instance_of(r, XBoolean)) {
		return this.compareWithBoolean(r, Operators.equals);
	}
	return this.compareWithNodeSet(r, Operators.equals);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.evaluate"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>evaluate (c)](#apidoc.element.xpath.XNodeSet.prototype.evaluate)
- description and source-code
```javascript
evaluate = function (c) {
	return this;
}
```
- example usage
```shell
...

Using the same interface you have on modern browsers ([MDN])

'''''javascript
var node = null;
var xml = "<book author='J. K. Rowling'><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var result = xpath.evaluate(
    "/book/title",            // xpathExpression
    doc,                        // contextNode
    null,                       // namespaceResolver
    xpath.XPathResult.ANY_TYPE, // resultType
    null                        // result
)
...
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.first"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>first ()](#apidoc.element.xpath.XNodeSet.prototype.first)
- description and source-code
```javascript
first = function () {
	var p = this.buildTree();
	if (p == null) {
		return null;
	}
	while (p.left != null) {
		p = p.left;
	}
	return p.node;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.greaterthan"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>greaterthan (r)](#apidoc.element.xpath.XNodeSet.prototype.greaterthan)
- description and source-code
```javascript
greaterthan = function (r) {
	if (Utilities.instance_of(r, XString)) {
		return this.compareWithNumber(r.number(), Operators.greaterthan);
	}
	if (Utilities.instance_of(r, XNumber)) {
		return this.compareWithNumber(r, Operators.greaterthan);
	}
	if (Utilities.instance_of(r, XBoolean)) {
		return this.compareWithBoolean(r, Operators.greaterthan);
	}
	return this.compareWithNodeSet(r, Operators.greaterthan);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.greaterthanorequal"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>greaterthanorequal (r)](#apidoc.element.xpath.XNodeSet.prototype.greaterthanorequal)
- description and source-code
```javascript
greaterthanorequal = function (r) {
	if (Utilities.instance_of(r, XString)) {
		return this.compareWithNumber(r.number(), Operators.greaterthanorequal);
	}
	if (Utilities.instance_of(r, XNumber)) {
		return this.compareWithNumber(r, Operators.greaterthanorequal);
	}
	if (Utilities.instance_of(r, XBoolean)) {
		return this.compareWithBoolean(r, Operators.greaterthanorequal);
	}
	return this.compareWithNodeSet(r, Operators.greaterthanorequal);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.init"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>init ()](#apidoc.element.xpath.XNodeSet.prototype.init)
- description and source-code
```javascript
init = function () {
    this.tree = null;
	this.nodes = [];
	this.size = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.lessthan"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>lessthan (r)](#apidoc.element.xpath.XNodeSet.prototype.lessthan)
- description and source-code
```javascript
lessthan = function (r) {
	if (Utilities.instance_of(r, XString)) {
		return this.compareWithNumber(r.number(), Operators.lessthan);
	}
	if (Utilities.instance_of(r, XNumber)) {
		return this.compareWithNumber(r, Operators.lessthan);
	}
	if (Utilities.instance_of(r, XBoolean)) {
		return this.compareWithBoolean(r, Operators.lessthan);
	}
	return this.compareWithNodeSet(r, Operators.lessthan);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.lessthanorequal"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>lessthanorequal (r)](#apidoc.element.xpath.XNodeSet.prototype.lessthanorequal)
- description and source-code
```javascript
lessthanorequal = function (r) {
	if (Utilities.instance_of(r, XString)) {
		return this.compareWithNumber(r.number(), Operators.lessthanorequal);
	}
	if (Utilities.instance_of(r, XNumber)) {
		return this.compareWithNumber(r, Operators.lessthanorequal);
	}
	if (Utilities.instance_of(r, XBoolean)) {
		return this.compareWithBoolean(r, Operators.lessthanorequal);
	}
	return this.compareWithNodeSet(r, Operators.lessthanorequal);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.nodeset"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>nodeset ()](#apidoc.element.xpath.XNodeSet.prototype.nodeset)
- description and source-code
```javascript
nodeset = function () {
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.notequal"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>notequal (r)](#apidoc.element.xpath.XNodeSet.prototype.notequal)
- description and source-code
```javascript
notequal = function (r) {
	if (Utilities.instance_of(r, XString)) {
		return this.compareWithString(r, Operators.notequal);
	}
	if (Utilities.instance_of(r, XNumber)) {
		return this.compareWithNumber(r, Operators.notequal);
	}
	if (Utilities.instance_of(r, XBoolean)) {
		return this.compareWithBoolean(r, Operators.notequal);
	}
	return this.compareWithNodeSet(r, Operators.notequal);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.number"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>number ()](#apidoc.element.xpath.XNodeSet.prototype.number)
- description and source-code
```javascript
number = function () {
	return new XNumber(this.string());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.numberValue"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>numberValue ()](#apidoc.element.xpath.XNodeSet.prototype.numberValue)
- description and source-code
```javascript
numberValue = function () {
	return Number(this.string());
}
```
- example usage
```shell
...
    return function (context, value) {
        assert.equal(2, arguments.length);
        var str = value.stringValue();
        return str + str;
    };
case "square":
    return function (context, value) {
        var num = value.numberValue();
        return num * num;
    };

case "xor":
    return function (context, l, r) {
        assert.equal(3, arguments.length);
        var lbool = l.booleanValue();
...
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.string"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>string ()](#apidoc.element.xpath.XNodeSet.prototype.string)
- description and source-code
```javascript
string = function () {
	return new XString(this.toString());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.stringForContainerNode"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>stringForContainerNode (n)](#apidoc.element.xpath.XNodeSet.prototype.stringForContainerNode)
- description and source-code
```javascript
stringForContainerNode = function (n) {
	var s = "";
	for (var n2 = n.firstChild; n2 != null; n2 = n2.nextSibling) {
        var nt = n2.nodeType;
        //  Element,    Text,       CDATA,      Document,   Document Fragment
        if (nt === 1 || nt === 3 || nt === 4 || nt === 9 || nt === 11) {
            s += this.stringForNode(n2);
        }
	}
	return s;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.stringForNode"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>stringForNode (n)](#apidoc.element.xpath.XNodeSet.prototype.stringForNode)
- description and source-code
```javascript
stringForNode = function (n) {
	if (n.nodeType == 9   /*Node.DOCUMENT_NODE*/ ||
        n.nodeType == 1   /*Node.ELEMENT_NODE */ ||
        n.nodeType === 11 /*Node.DOCUMENT_FRAGMENT*/) {
		return this.stringForContainerNode(n);
	}
    if (n.nodeType === 2 /* Node.ATTRIBUTE_NODE */) {
        return n.value || n.nodeValue;
    }
	if (n.isNamespaceNode) {
		return n.namespace;
	}
	return n.nodeValue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.stringValue"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>stringValue ()](#apidoc.element.xpath.XNodeSet.prototype.stringValue)
- description and source-code
```javascript
stringValue = function () {
	return this.toString();
}
```
- example usage
```shell
...
		var xml = '<book><title>Harry Potter</title></book>';
var doc = new dom().parseFromString(xml);

var parsed = xpath.parse('concat(double(/*/title), " is cool")');

function doubleString(context, value) {
    assert.equal(2, arguments.length);
    var str = value.stringValue();
    return str + str;
}

function functions(name, namespace) {
    if(name === 'double') {
        return doubleString;
    }
...
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.toArray"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>toArray ()](#apidoc.element.xpath.XNodeSet.prototype.toArray)
- description and source-code
```javascript
toArray = function () {
	var a = [];
	this.toArrayRec(this.buildTree(), a);
	return a;
}
```
- example usage
```shell
...
                    var lbool = l.booleanValue();
                    var rbool = r.booleanValue();
                    return (lbool || rbool) && !(lbool && rbool);
                };

            case "second":
                return function (context, nodes) {
                    var nodesArr = nodes.toArray();
                    var second = nodesArr[1];
                    return second ? [second] : [];
                };
        }
    }
    return null;
}
...
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.toArrayRec"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>toArrayRec (t, a)](#apidoc.element.xpath.XNodeSet.prototype.toArrayRec)
- description and source-code
```javascript
toArrayRec = function (t, a) {
	if (t != null) {
		this.toArrayRec(t.left, a);
		a.push(t.node);
		this.toArrayRec(t.right, a);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.toString"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>toString ()](#apidoc.element.xpath.XNodeSet.prototype.toString)
- description and source-code
```javascript
toString = function () {
	var p = this.first();
	if (p == null) {
		return "";
	}
	return this.stringForNode(p);
}
```
- example usage
```shell
...
  , dom = require('xmldom').DOMParser

var xml = "<book><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var nodes = xpath.select("//title", doc)

console.log(nodes[0].localName + ": " + nodes[0].firstChild.data)
console.log("Node: " + nodes[0].toString())
'''''
➡

    title: Harry Potter
    Node: <title>Harry Potter</title>

### Alternatively
...
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.toUnsortedArray"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>toUnsortedArray ()](#apidoc.element.xpath.XNodeSet.prototype.toUnsortedArray)
- description and source-code
```javascript
toUnsortedArray = function () {
    return this.nodes.slice();
}
```
- example usage
```shell
...
}

,"node set sorted and unsorted arrays": function (test) {
    var doc = new dom().parseFromString('<book><character>Harry</character><character>Ron</character><character>Hermione</character
></book>'),
        path = xpath.parse("/*/*[3] | /*/*[2] | /*/*[1]")
        nset = path.evaluateNodeSet({ node: doc }),
        sorted = nset.toArray(),
        unsorted = nset.toUnsortedArray();

    assert.equal(sorted.length, 3);
    assert.equal(unsorted.length, 3);

    assert.equal(sorted[0].textContent, 'Harry');
    assert.equal(sorted[1].textContent, 'Ron');
    assert.equal(sorted[2].textContent, 'Hermione');
...
```

#### <a name="apidoc.element.xpath.XNodeSet.prototype.union"></a>[function <span class="apidocSignatureSpan">xpath.XNodeSet.prototype.</span>union (r)](#apidoc.element.xpath.XNodeSet.prototype.union)
- description and source-code
```javascript
union = function (r) {
	var ns = new XNodeSet();
    ns.addArray(this.toUnsortedArray());
	ns.addArray(r.toUnsortedArray());
	return ns;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XNumber"></a>[module xpath.XNumber](#apidoc.module.xpath.XNumber)

#### <a name="apidoc.element.xpath.XNumber.XNumber"></a>[function <span class="apidocSignatureSpan">xpath.</span>XNumber (n)](#apidoc.element.xpath.XNumber.XNumber)
- description and source-code
```javascript
function XNumber(n) {
	if (arguments.length > 0) {
		this.init(n);
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XNumber.prototype"></a>[module xpath.XNumber.prototype](#apidoc.module.xpath.XNumber.prototype)

#### <a name="apidoc.element.xpath.XNumber.prototype.bool"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>bool ()](#apidoc.element.xpath.XNumber.prototype.bool)
- description and source-code
```javascript
bool = function () {
	return new XBoolean(this.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.booleanValue"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>booleanValue ()](#apidoc.element.xpath.XNumber.prototype.booleanValue)
- description and source-code
```javascript
booleanValue = function () {
	return this.bool().booleanValue();
}
```
- example usage
```shell
...
        var num = value.numberValue();
        return num * num;
    };

case "xor":
    return function (context, l, r) {
        assert.equal(3, arguments.length);
        var lbool = l.booleanValue();
        var rbool = r.booleanValue();
        return (lbool || rbool) && !(lbool && rbool);
    };

case "second":
    return function (context, nodes) {
        var nodesArr = nodes.toArray();
...
```

#### <a name="apidoc.element.xpath.XNumber.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>constructor (n)](#apidoc.element.xpath.XNumber.prototype.constructor)
- description and source-code
```javascript
function XNumber(n) {
	if (arguments.length > 0) {
		this.init(n);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.div"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>div (r)](#apidoc.element.xpath.XNumber.prototype.div)
- description and source-code
```javascript
div = function (r) {
	return new XNumber(this.num / r.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.equals"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>equals (r)](#apidoc.element.xpath.XNumber.prototype.equals)
- description and source-code
```javascript
equals = function (r) {
	if (Utilities.instance_of(r, XBoolean)) {
		return this.bool().equals(r);
	}
	if (Utilities.instance_of(r, XString)) {
		return this.equals(r.number());
	}
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this, Operators.equals);
	}
	return new XBoolean(this.num == r.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.evaluate"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>evaluate (c)](#apidoc.element.xpath.XNumber.prototype.evaluate)
- description and source-code
```javascript
evaluate = function (c) {
	return this;
}
```
- example usage
```shell
...

Using the same interface you have on modern browsers ([MDN])

'''''javascript
var node = null;
var xml = "<book author='J. K. Rowling'><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var result = xpath.evaluate(
    "/book/title",            // xpathExpression
    doc,                        // contextNode
    null,                       // namespaceResolver
    xpath.XPathResult.ANY_TYPE, // resultType
    null                        // result
)
...
```

#### <a name="apidoc.element.xpath.XNumber.prototype.greaterthan"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>greaterthan (r)](#apidoc.element.xpath.XNumber.prototype.greaterthan)
- description and source-code
```javascript
greaterthan = function (r) {
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this, Operators.lessthanorequal);
	}
	if (Utilities.instance_of(r, XBoolean) || Utilities.instance_of(r, XString)) {
		return this.greaterthan(r.number());
	}
	return new XBoolean(this.num > r.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.greaterthanorequal"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>greaterthanorequal (r)](#apidoc.element.xpath.XNumber.prototype.greaterthanorequal)
- description and source-code
```javascript
greaterthanorequal = function (r) {
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this, Operators.lessthan);
	}
	if (Utilities.instance_of(r, XBoolean) || Utilities.instance_of(r, XString)) {
		return this.greaterthanorequal(r.number());
	}
	return new XBoolean(this.num >= r.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.init"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>init (n)](#apidoc.element.xpath.XNumber.prototype.init)
- description and source-code
```javascript
init = function (n) {
	this.num = typeof n === "string" ? this.parse(n) : Number(n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.lessthan"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>lessthan (r)](#apidoc.element.xpath.XNumber.prototype.lessthan)
- description and source-code
```javascript
lessthan = function (r) {
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this, Operators.greaterthanorequal);
	}
	if (Utilities.instance_of(r, XBoolean) || Utilities.instance_of(r, XString)) {
		return this.lessthan(r.number());
	}
	return new XBoolean(this.num < r.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.lessthanorequal"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>lessthanorequal (r)](#apidoc.element.xpath.XNumber.prototype.lessthanorequal)
- description and source-code
```javascript
lessthanorequal = function (r) {
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this, Operators.greaterthan);
	}
	if (Utilities.instance_of(r, XBoolean) || Utilities.instance_of(r, XString)) {
		return this.lessthanorequal(r.number());
	}
	return new XBoolean(this.num <= r.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.minus"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>minus (r)](#apidoc.element.xpath.XNumber.prototype.minus)
- description and source-code
```javascript
minus = function (r) {
	return new XNumber(this.num - r.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.mod"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>mod (r)](#apidoc.element.xpath.XNumber.prototype.mod)
- description and source-code
```javascript
mod = function (r) {
	return new XNumber(this.num % r.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.multiply"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>multiply (r)](#apidoc.element.xpath.XNumber.prototype.multiply)
- description and source-code
```javascript
multiply = function (r) {
	return new XNumber(this.num * r.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.negate"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>negate ()](#apidoc.element.xpath.XNumber.prototype.negate)
- description and source-code
```javascript
negate = function () {
	return new XNumber(-this.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.nodeset"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>nodeset ()](#apidoc.element.xpath.XNumber.prototype.nodeset)
- description and source-code
```javascript
nodeset = function () {
	throw new Error("Cannot convert number to nodeset");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.notequal"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>notequal (r)](#apidoc.element.xpath.XNumber.prototype.notequal)
- description and source-code
```javascript
notequal = function (r) {
	if (Utilities.instance_of(r, XBoolean)) {
		return this.bool().notequal(r);
	}
	if (Utilities.instance_of(r, XString)) {
		return this.notequal(r.number());
	}
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this, Operators.notequal);
	}
	return new XBoolean(this.num != r.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.number"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>number ()](#apidoc.element.xpath.XNumber.prototype.number)
- description and source-code
```javascript
number = function () {
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.numberValue"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>numberValue ()](#apidoc.element.xpath.XNumber.prototype.numberValue)
- description and source-code
```javascript
numberValue = function () {
	return this.num;
}
```
- example usage
```shell
...
    return function (context, value) {
        assert.equal(2, arguments.length);
        var str = value.stringValue();
        return str + str;
    };
case "square":
    return function (context, value) {
        var num = value.numberValue();
        return num * num;
    };

case "xor":
    return function (context, l, r) {
        assert.equal(3, arguments.length);
        var lbool = l.booleanValue();
...
```

#### <a name="apidoc.element.xpath.XNumber.prototype.parse"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>parse (s)](#apidoc.element.xpath.XNumber.prototype.parse)
- description and source-code
```javascript
parse = function (s) {
    // XPath representation of numbers is more restrictive than what Number() or parseFloat() allow
    return this.numberFormat.test(s) ? parseFloat(s) : Number.NaN;
}
```
- example usage
```shell
...
		assert.ok(Number.isNaN(xpath.select('number("2e9")')), 'number("2e9")');
		assert.ok(Number.isNaN(xpath.select('number("+33")')), 'number("+33")');
		
		test.done();
	}
	
	,'correct number to string conversion': function (test) {
		assert.equal('0.0000000000000000000000005250000000000001', xpath.parse('0.525 div 1000000 div 1000000 div 1000000 div 1000000').
evaluateString());
		assert.equal('525000000000000000000000', xpath.parse('0.525 * 1000000 * 1000000 * 1000000 * 1000000').evaluateString());
		
		test.done();
	}
	
	,'local-name() and name() of processing instruction': function (test) {
	    var xml = '<?book-record added="2015-01-16" author="J.K. Rowling" ?><book>Harry Potter</book>';
...
```

#### <a name="apidoc.element.xpath.XNumber.prototype.plus"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>plus (r)](#apidoc.element.xpath.XNumber.prototype.plus)
- description and source-code
```javascript
plus = function (r) {
	return new XNumber(this.num + r.num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.string"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>string ()](#apidoc.element.xpath.XNumber.prototype.string)
- description and source-code
```javascript
string = function () {
	
	
	return new XString(this.toString());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XNumber.prototype.stringValue"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>stringValue ()](#apidoc.element.xpath.XNumber.prototype.stringValue)
- description and source-code
```javascript
stringValue = function () {
	return this.string().stringValue();
}
```
- example usage
```shell
...
		var xml = '<book><title>Harry Potter</title></book>';
var doc = new dom().parseFromString(xml);

var parsed = xpath.parse('concat(double(/*/title), " is cool")');

function doubleString(context, value) {
    assert.equal(2, arguments.length);
    var str = value.stringValue();
    return str + str;
}

function functions(name, namespace) {
    if(name === 'double') {
        return doubleString;
    }
...
```

#### <a name="apidoc.element.xpath.XNumber.prototype.toString"></a>[function <span class="apidocSignatureSpan">xpath.XNumber.prototype.</span>toString ()](#apidoc.element.xpath.XNumber.prototype.toString)
- description and source-code
```javascript
toString = function () {
	var strValue = this.num.toString();

	if (strValue.indexOf('e-') !== -1) {
		return padSmallNumber(strValue);
	}

	if (strValue.indexOf('e') !== -1) {
		return padLargeNumber(strValue);
	}
	
	return strValue;
}
```
- example usage
```shell
...
  , dom = require('xmldom').DOMParser

var xml = "<book><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var nodes = xpath.select("//title", doc)

console.log(nodes[0].localName + ": " + nodes[0].firstChild.data)
console.log("Node: " + nodes[0].toString())
'''''
➡

    title: Harry Potter
    Node: <title>Harry Potter</title>

### Alternatively
...
```



# <a name="apidoc.module.xpath.XPath"></a>[module xpath.XPath](#apidoc.module.xpath.XPath)

#### <a name="apidoc.element.xpath.XPath.XPath"></a>[function <span class="apidocSignatureSpan">xpath.</span>XPath (e)](#apidoc.element.xpath.XPath.XPath)
- description and source-code
```javascript
function XPath(e) {
	this.expression = e;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XPath.prototype"></a>[module xpath.XPath.prototype](#apidoc.module.xpath.XPath.prototype)

#### <a name="apidoc.element.xpath.XPath.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.XPath.prototype.</span>constructor (e)](#apidoc.element.xpath.XPath.prototype.constructor)
- description and source-code
```javascript
function XPath(e) {
	this.expression = e;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XPath.prototype.evaluate"></a>[function <span class="apidocSignatureSpan">xpath.XPath.prototype.</span>evaluate (c)](#apidoc.element.xpath.XPath.prototype.evaluate)
- description and source-code
```javascript
evaluate = function (c) {
	c.contextNode = c.expressionContextNode;
	c.contextSize = 1;
	c.contextPosition = 1;
	c.caseInsensitive = false;
	if (c.contextNode != null) {
		var doc = c.contextNode;
		if (doc.nodeType != 9 /*Node.DOCUMENT_NODE*/) {
			doc = doc.ownerDocument;
		}
		try {
			c.caseInsensitive = doc.implementation.hasFeature("HTML", "2.0");
		} catch (e) {
			c.caseInsensitive = true;
		}
	}
	return this.expression.evaluate(c);
}
```
- example usage
```shell
...

Using the same interface you have on modern browsers ([MDN])

'''''javascript
var node = null;
var xml = "<book author='J. K. Rowling'><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var result = xpath.evaluate(
    "/book/title",            // xpathExpression
    doc,                        // contextNode
    null,                       // namespaceResolver
    xpath.XPathResult.ANY_TYPE, // resultType
    null                        // result
)
...
```

#### <a name="apidoc.element.xpath.XPath.prototype.toString"></a>[function <span class="apidocSignatureSpan">xpath.XPath.prototype.</span>toString ()](#apidoc.element.xpath.XPath.prototype.toString)
- description and source-code
```javascript
toString = function () {
	return this.expression.toString();
}
```
- example usage
```shell
...
  , dom = require('xmldom').DOMParser

var xml = "<book><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var nodes = xpath.select("//title", doc)

console.log(nodes[0].localName + ": " + nodes[0].firstChild.data)
console.log("Node: " + nodes[0].toString())
'''''
➡

    title: Harry Potter
    Node: <title>Harry Potter</title>

### Alternatively
...
```



# <a name="apidoc.module.xpath.XPathContext"></a>[module xpath.XPathContext](#apidoc.module.xpath.XPathContext)

#### <a name="apidoc.element.xpath.XPathContext.XPathContext"></a>[function <span class="apidocSignatureSpan">xpath.</span>XPathContext (vr, nr, fr)](#apidoc.element.xpath.XPathContext.XPathContext)
- description and source-code
```javascript
function XPathContext(vr, nr, fr) {
	this.variableResolver = vr != null ? vr : new VariableResolver();
	this.namespaceResolver = nr != null ? nr : new NamespaceResolver();
	this.functionResolver = fr != null ? fr : new FunctionResolver();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XPathContext.prototype"></a>[module xpath.XPathContext.prototype](#apidoc.module.xpath.XPathContext.prototype)

#### <a name="apidoc.element.xpath.XPathContext.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.XPathContext.prototype.</span>constructor (vr, nr, fr)](#apidoc.element.xpath.XPathContext.prototype.constructor)
- description and source-code
```javascript
function XPathContext(vr, nr, fr) {
	this.variableResolver = vr != null ? vr : new VariableResolver();
	this.namespaceResolver = nr != null ? nr : new NamespaceResolver();
	this.functionResolver = fr != null ? fr : new FunctionResolver();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XPathParser"></a>[module xpath.XPathParser](#apidoc.module.xpath.XPathParser)

#### <a name="apidoc.element.xpath.XPathParser.XPathParser"></a>[function <span class="apidocSignatureSpan">xpath.</span>XPathParser ()](#apidoc.element.xpath.XPathParser.XPathParser)
- description and source-code
```javascript
function XPathParser() {
	this.init();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XPathParser.prototype"></a>[module xpath.XPathParser.prototype](#apidoc.module.xpath.XPathParser.prototype)

#### <a name="apidoc.element.xpath.XPathParser.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.XPathParser.prototype.</span>constructor ()](#apidoc.element.xpath.XPathParser.prototype.constructor)
- description and source-code
```javascript
function XPathParser() {
	this.init();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XPathParser.prototype.init"></a>[function <span class="apidocSignatureSpan">xpath.XPathParser.prototype.</span>init ()](#apidoc.element.xpath.XPathParser.prototype.init)
- description and source-code
```javascript
init = function () {
	this.reduceActions = [];

	this.reduceActions[3] = function(rhs) {
		return new OrOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[5] = function(rhs) {
		return new AndOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[7] = function(rhs) {
		return new EqualsOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[8] = function(rhs) {
		return new NotEqualOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[10] = function(rhs) {
		return new LessThanOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[11] = function(rhs) {
		return new GreaterThanOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[12] = function(rhs) {
		return new LessThanOrEqualOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[13] = function(rhs) {
		return new GreaterThanOrEqualOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[15] = function(rhs) {
		return new PlusOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[16] = function(rhs) {
		return new MinusOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[18] = function(rhs) {
		return new MultiplyOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[19] = function(rhs) {
		return new DivOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[20] = function(rhs) {
		return new ModOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[22] = function(rhs) {
		return new UnaryMinusOperation(rhs[1]);
	};
	this.reduceActions[24] = function(rhs) {
		return new BarOperation(rhs[0], rhs[2]);
	};
	this.reduceActions[25] = function(rhs) {
		return new PathExpr(undefined, undefined, rhs[0]);
	};
	this.reduceActions[27] = function(rhs) {
		rhs[0].locationPath = rhs[2];
		return rhs[0];
	};
	this.reduceActions[28] = function(rhs) {
		rhs[0].locationPath = rhs[2];
		rhs[0].locationPath.steps.unshift(new Step(Step.DESCENDANTORSELF, new NodeTest(NodeTest.NODE, undefined), []));
		return rhs[0];
	};
	this.reduceActions[29] = function(rhs) {
		return new PathExpr(rhs[0], [], undefined);
	};
	this.reduceActions[30] = function(rhs) {
		if (Utilities.instance_of(rhs[0], PathExpr)) {
			if (rhs[0].filterPredicates == undefined) {
				rhs[0].filterPredicates = [];
			}
			rhs[0].filterPredicates.push(rhs[1]);
			return rhs[0];
		} else {
			return new PathExpr(rhs[0], [rhs[1]], undefined);
		}
	};
	this.reduceActions[32] = function(rhs) {
		return rhs[1];
	};
	this.reduceActions[33] = function(rhs) {
		return new XString(rhs[0]);
	};
	this.reduceActions[34] = function(rhs) {
		return new XNumber(rhs[0]);
	};
	this.reduceActions[36] = function(rhs) {
		return new FunctionCall(rhs[0], []);
	};
	this.reduceActions[37] = function(rhs) {
		return new FunctionCall(rhs[0], rhs[2]);
	};
	this.reduceActions[38] = function(rhs) {
		return [ rhs[0] ];
	};
	this.reduceActions[39] = function(rhs) {
		rhs[2].unshift(rhs[0]);
		return rhs[2];
	};
	this.reduceActions[43] = function(rhs) {
		return new LocationPath(true, []);
	};
	this.reduceActions[44] = function(rhs) {
		rhs[1].absolute = true;
		return rhs[1];
	};
	this.reduceActions[46] = function(rhs) {
		return new LocationPath(false, [ rhs[0] ]);
	};
	this.reduceActions[47] = function(rhs) {
		rhs[0].steps.push(rhs[2]);
		return rhs[0];
	};
	this.reduceActions[49] = function(rhs) {
		return new Step(rhs[0], rhs[1], []);
	};
	this.reduceActions[50] = function(rhs) {
		return new Step(Step.CHILD, rhs[0], []);
	};
	this.reduceActions[51] = function(rhs) {
		return new Step(rhs[0], rhs[1], rhs[2]);
	};
	this.reduceActions[52] = function(rhs) {
		return new Step(Step.CHILD, rhs[0], rhs[1]);
	};
	this.reduceActions[54] = function(rhs) {
		return [ rhs[0] ];
	};
	this.reduceActions[55] = function(rhs) {
		rhs[1].unshift(rhs[0]);
		return rhs[1];
	};
	this.reduceActions[56] = function(rhs) {
		if (rhs[0] == "ancestor") {
			return Step.ANCESTOR;
		} else if (rhs[0] == "ancestor-or-self") {
			return Step.ANCESTORORSELF;
		} else if (rhs[0] == "attribute") {
			return Step.ATTRIBUTE;
		} else if (rhs[0] == "child") {
			return Step.CHILD;
		} else if (rhs[0] == ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XPathParser.prototype.parse"></a>[function <span class="apidocSignatureSpan">xpath.XPathParser.prototype.</span>parse (s)](#apidoc.element.xpath.XPathParser.prototype.parse)
- description and source-code
```javascript
parse = function (s) {
	var types;
	var values;
	var res = this.tokenize(s);
	if (res == undefined) {
		return undefined;
	}
	types = res[0];
	values = res[1];
	var tokenPos = 0;
	var state = [];
	var tokenType = [];
	var tokenValue = [];
	var s;
	var a;
	var t;

	state.push(0);
	tokenType.push(1);
	tokenValue.push("_S");

	a = types[tokenPos];
	t = values[tokenPos++];
	while (1) {
		s = state[state.length - 1];
		switch (XPathParser.actionTable[s].charAt(a - 1)) {
			case XPathParser.SHIFT:
				tokenType.push(-a);
				tokenValue.push(t);
				state.push(XPathParser.actionTableNumber[s].charCodeAt(a - 1) - 32);
				a = types[tokenPos];
				t = values[tokenPos++];
				break;
			case XPathParser.REDUCE:
				var num = XPathParser.productions[XPathParser.actionTableNumber[s].charCodeAt(a - 1) - 32][1];
				var rhs = [];
				for (var i = 0; i < num; i++) {
					tokenType.pop();
					rhs.unshift(tokenValue.pop());
					state.pop();
				}
				var s_ = state[state.length - 1];
				tokenType.push(XPathParser.productions[XPathParser.actionTableNumber[s].charCodeAt(a - 1) - 32][0]);
				if (this.reduceActions[XPathParser.actionTableNumber[s].charCodeAt(a - 1) - 32] == undefined) {
					tokenValue.push(rhs[0]);
				} else {
					tokenValue.push(this.reduceActions[XPathParser.actionTableNumber[s].charCodeAt(a - 1) - 32](rhs));
				}
				state.push(XPathParser.gotoTable[s_].charCodeAt(XPathParser.productions[XPathParser.actionTableNumber[s].charCodeAt(a - 1) -
32][0] - 2) - 33);
				break;
			case XPathParser.ACCEPT:
				return new XPath(tokenValue.pop());
			default:
				throw new Error("XPath parse error");
		}
	}
}
```
- example usage
```shell
...
		assert.ok(Number.isNaN(xpath.select('number("2e9")')), 'number("2e9")');
		assert.ok(Number.isNaN(xpath.select('number("+33")')), 'number("+33")');
		
		test.done();
	}
	
	,'correct number to string conversion': function (test) {
		assert.equal('0.0000000000000000000000005250000000000001', xpath.parse('0.525 div 1000000 div 1000000 div 1000000 div 1000000').
evaluateString());
		assert.equal('525000000000000000000000', xpath.parse('0.525 * 1000000 * 1000000 * 1000000 * 1000000').evaluateString());
		
		test.done();
	}
	
	,'local-name() and name() of processing instruction': function (test) {
	    var xml = '<?book-record added="2015-01-16" author="J.K. Rowling" ?><book>Harry Potter</book>';
...
```

#### <a name="apidoc.element.xpath.XPathParser.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">xpath.XPathParser.prototype.</span>tokenize (s1)](#apidoc.element.xpath.XPathParser.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (s1) {
	var types = [];
	var values = [];
	var s = s1 + '\0';

	var pos = 0;
	var c = s.charAt(pos++);
	while (1) {
		while (c == ' ' || c == '\t' || c == '\r' || c == '\n') {
			c = s.charAt(pos++);
		}
		if (c == '\0' || pos >= s.length) {
			break;
		}

		if (c == '(') {
			types.push(XPathParser.LEFTPARENTHESIS);
			values.push(c);
			c = s.charAt(pos++);
			continue;
		}
		if (c == ')') {
			types.push(XPathParser.RIGHTPARENTHESIS);
			values.push(c);
			c = s.charAt(pos++);
			continue;
		}
		if (c == '[') {
			types.push(XPathParser.LEFTBRACKET);
			values.push(c);
			c = s.charAt(pos++);
			continue;
		}
		if (c == ']') {
			types.push(XPathParser.RIGHTBRACKET);
			values.push(c);
			c = s.charAt(pos++);
			continue;
		}
		if (c == '@') {
			types.push(XPathParser.AT);
			values.push(c);
			c = s.charAt(pos++);
			continue;
		}
		if (c == ',') {
			types.push(XPathParser.COMMA);
			values.push(c);
			c = s.charAt(pos++);
			continue;
		}
		if (c == '|') {
			types.push(XPathParser.BAR);
			values.push(c);
			c = s.charAt(pos++);
			continue;
		}
		if (c == '+') {
			types.push(XPathParser.PLUS);
			values.push(c);
			c = s.charAt(pos++);
			continue;
		}
		if (c == '-') {
			types.push(XPathParser.MINUS);
			values.push(c);
			c = s.charAt(pos++);
			continue;
		}
		if (c == '=') {
			types.push(XPathParser.EQUALS);
			values.push(c);
			c = s.charAt(pos++);
			continue;
		}
		if (c == '$') {
			types.push(XPathParser.DOLLAR);
			values.push(c);
			c = s.charAt(pos++);
			continue;
		}

		if (c == '.') {
			c = s.charAt(pos++);
			if (c == '.') {
				types.push(XPathParser.DOUBLEDOT);
				values.push("..");
				c = s.charAt(pos++);
				continue;
			}
			if (c >= '0' && c <= '9') {
				var number = "." + c;
				c = s.charAt(pos++);
				while (c >= '0' && c <= '9') {
					number += c;
					c = s.charAt(pos++);
				}
				types.push(XPathParser.NUMBER);
				values.push(number);
				continue;
			}
			types.push(XPathParser.DOT);
			values.push('.');
			continue;
		}

		if (c == '\'' || c == '"') {
			var delimiter = c;
			var literal = "";
			while (pos < s.length && (c = s.charAt(pos)) !== delimiter) {
				literal += c;
                pos += 1;
			}
            if (c !== delimiter) {
                throw XPathException.fromMessage("Unterminated string literal: " + delimiter + literal);
            }
            pos += 1;
			types.push(XPathParser.LITERAL);
			values.push(literal);
			c = s.charAt(pos++);
			continue;
		}

		if (c >= '0' && c <= '9') {
			var number = c;
			c = s.charAt(pos++);
			while (c >= '0' && c <= '9') {
				number += c;
				c = s.charAt(pos++);
			}
			if (c == '.') {
				if (s.charAt(pos) >= '0' && s.charAt(pos) <= '9') {
					number += c;
					number += s.charAt(pos++);
					c = s.charAt(pos++);
					while (c >= '0' && c <= '9') {
						number += c;
						c = s.charAt(pos++);
					}
				}
			}
			types.push(XPathParser.NUMBER);
			values.push(number);
			continue;
		}

		if (c == '*') {
			if (types.length > 0) {
				var last = types[types.length - 1];
				if (last != XPathParser.AT
						&& last != XPathParser.DOUBLECOLON
						&& last != XPathParser.LEFTPARENTHESIS
						&& last != XPathParser.LEFTBRACKET
						&& last != XPathParser.AND
						&& last != XPathParser.OR
						&& last != XPathParser.MOD
						&& last != XPathParser.DIV
						&& last != XPathParser.MULTIPLYOPERATOR
						&& last != XPathParser.SLASH
						&& last != XPathParser.DOUBLESLASH
						&& last != XPathParser.BAR
						&& last != XPathParser.PLUS
						&& last != XPathParser.MINUS
						&& last != XPathParser.EQUALS
						&& last != XPathParser.NOTEQUAL
						&& last != XPathParser.LESSTHAN
						&& last != XPathParser.LESSTHANOREQUAL
						&& last != XPathParser.GREATERTHAN
						&& last != XPathParser.GREATERTHANOREQUAL) {
					types.push(XPathParser.MULTIPLYOPERATOR);
					values.push(c);
					c = s.charAt(pos++);
					continue; ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XPathResult"></a>[module xpath.XPathResult](#apidoc.module.xpath.XPathResult)

#### <a name="apidoc.element.xpath.XPathResult.XPathResult"></a>[function <span class="apidocSignatureSpan">xpath.</span>XPathResult (v, t)](#apidoc.element.xpath.XPathResult.XPathResult)
- description and source-code
```javascript
function XPathResult(v, t) {
	if (t == XPathResult.ANY_TYPE) {
		if (v.constructor === XString) {
			t = XPathResult.STRING_TYPE;
		} else if (v.constructor === XNumber) {
			t = XPathResult.NUMBER_TYPE;
		} else if (v.constructor === XBoolean) {
			t = XPathResult.BOOLEAN_TYPE;
		} else if (v.constructor === XNodeSet) {
			t = XPathResult.UNORDERED_NODE_ITERATOR_TYPE;
		}
	}
	this.resultType = t;
	switch (t) {
		case XPathResult.NUMBER_TYPE:
			this.numberValue = v.numberValue();
			return;
		case XPathResult.STRING_TYPE:
			this.stringValue = v.stringValue();
			return;
		case XPathResult.BOOLEAN_TYPE:
			this.booleanValue = v.booleanValue();
			return;
		case XPathResult.ANY_UNORDERED_NODE_TYPE:
		case XPathResult.FIRST_ORDERED_NODE_TYPE:
			if (v.constructor === XNodeSet) {
				this.singleNodeValue = v.first();
				return;
			}
			break;
		case XPathResult.UNORDERED_NODE_ITERATOR_TYPE:
		case XPathResult.ORDERED_NODE_ITERATOR_TYPE:
			if (v.constructor === XNodeSet) {
				this.invalidIteratorState = false;
				this.nodes = v.toArray();
				this.iteratorIndex = 0;
				return;
			}
			break;
		case XPathResult.UNORDERED_NODE_SNAPSHOT_TYPE:
		case XPathResult.ORDERED_NODE_SNAPSHOT_TYPE:
			if (v.constructor === XNodeSet) {
				this.nodes = v.toArray();
				this.snapshotLength = this.nodes.length;
				return;
			}
			break;
	}
	throw new XPathException(XPathException.TYPE_ERR);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XPathResult.prototype"></a>[module xpath.XPathResult.prototype](#apidoc.module.xpath.XPathResult.prototype)

#### <a name="apidoc.element.xpath.XPathResult.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.XPathResult.prototype.</span>constructor (v, t)](#apidoc.element.xpath.XPathResult.prototype.constructor)
- description and source-code
```javascript
function XPathResult(v, t) {
	if (t == XPathResult.ANY_TYPE) {
		if (v.constructor === XString) {
			t = XPathResult.STRING_TYPE;
		} else if (v.constructor === XNumber) {
			t = XPathResult.NUMBER_TYPE;
		} else if (v.constructor === XBoolean) {
			t = XPathResult.BOOLEAN_TYPE;
		} else if (v.constructor === XNodeSet) {
			t = XPathResult.UNORDERED_NODE_ITERATOR_TYPE;
		}
	}
	this.resultType = t;
	switch (t) {
		case XPathResult.NUMBER_TYPE:
			this.numberValue = v.numberValue();
			return;
		case XPathResult.STRING_TYPE:
			this.stringValue = v.stringValue();
			return;
		case XPathResult.BOOLEAN_TYPE:
			this.booleanValue = v.booleanValue();
			return;
		case XPathResult.ANY_UNORDERED_NODE_TYPE:
		case XPathResult.FIRST_ORDERED_NODE_TYPE:
			if (v.constructor === XNodeSet) {
				this.singleNodeValue = v.first();
				return;
			}
			break;
		case XPathResult.UNORDERED_NODE_ITERATOR_TYPE:
		case XPathResult.ORDERED_NODE_ITERATOR_TYPE:
			if (v.constructor === XNodeSet) {
				this.invalidIteratorState = false;
				this.nodes = v.toArray();
				this.iteratorIndex = 0;
				return;
			}
			break;
		case XPathResult.UNORDERED_NODE_SNAPSHOT_TYPE:
		case XPathResult.ORDERED_NODE_SNAPSHOT_TYPE:
			if (v.constructor === XNodeSet) {
				this.nodes = v.toArray();
				this.snapshotLength = this.nodes.length;
				return;
			}
			break;
	}
	throw new XPathException(XPathException.TYPE_ERR);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XPathResult.prototype.iterateNext"></a>[function <span class="apidocSignatureSpan">xpath.XPathResult.prototype.</span>iterateNext ()](#apidoc.element.xpath.XPathResult.prototype.iterateNext)
- description and source-code
```javascript
iterateNext = function () {
	if (this.resultType != XPathResult.UNORDERED_NODE_ITERATOR_TYPE
			&& this.resultType != XPathResult.ORDERED_NODE_ITERATOR_TYPE) {
		throw new XPathException(XPathException.TYPE_ERR);
	}
	return this.nodes[this.iteratorIndex++];
}
```
- example usage
```shell
...
    "/book/title",            // xpathExpression
    doc,                        // contextNode
    null,                       // namespaceResolver
    xpath.XPathResult.ANY_TYPE, // resultType
    null                        // result
)

node = result.iterateNext();
while (node) {
    console.log(node.localName + ": " + node.firstChild.data);
    console.log("Node: " + node.toString());

    node = result.iterateNext();
}
'''''
...
```

#### <a name="apidoc.element.xpath.XPathResult.prototype.snapshotItem"></a>[function <span class="apidocSignatureSpan">xpath.XPathResult.prototype.</span>snapshotItem (i)](#apidoc.element.xpath.XPathResult.prototype.snapshotItem)
- description and source-code
```javascript
snapshotItem = function (i) {
	if (this.resultType != XPathResult.UNORDERED_NODE_SNAPSHOT_TYPE
			&& this.resultType != XPathResult.ORDERED_NODE_SNAPSHOT_TYPE) {
		throw new XPathException(XPathException.TYPE_ERR);
	}
	return this.nodes[i];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XString"></a>[module xpath.XString](#apidoc.module.xpath.XString)

#### <a name="apidoc.element.xpath.XString.XString"></a>[function <span class="apidocSignatureSpan">xpath.</span>XString (s)](#apidoc.element.xpath.XString.XString)
- description and source-code
```javascript
function XString(s) {
	if (arguments.length > 0) {
		this.init(s);
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xpath.XString.prototype"></a>[module xpath.XString.prototype](#apidoc.module.xpath.XString.prototype)

#### <a name="apidoc.element.xpath.XString.prototype.bool"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>bool ()](#apidoc.element.xpath.XString.prototype.bool)
- description and source-code
```javascript
bool = function () {
	return new XBoolean(this.str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString.prototype.booleanValue"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>booleanValue ()](#apidoc.element.xpath.XString.prototype.booleanValue)
- description and source-code
```javascript
booleanValue = function () {
	return this.bool().booleanValue();
}
```
- example usage
```shell
...
        var num = value.numberValue();
        return num * num;
    };

case "xor":
    return function (context, l, r) {
        assert.equal(3, arguments.length);
        var lbool = l.booleanValue();
        var rbool = r.booleanValue();
        return (lbool || rbool) && !(lbool && rbool);
    };

case "second":
    return function (context, nodes) {
        var nodesArr = nodes.toArray();
...
```

#### <a name="apidoc.element.xpath.XString.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>constructor (s)](#apidoc.element.xpath.XString.prototype.constructor)
- description and source-code
```javascript
function XString(s) {
	if (arguments.length > 0) {
		this.init(s);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString.prototype.equals"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>equals (r)](#apidoc.element.xpath.XString.prototype.equals)
- description and source-code
```javascript
equals = function (r) {
	if (Utilities.instance_of(r, XBoolean)) {
		return this.bool().equals(r);
	}
	if (Utilities.instance_of(r, XNumber)) {
		return this.number().equals(r);
	}
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithString(this, Operators.equals);
	}
	return new XBoolean(this.str == r.str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString.prototype.evaluate"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>evaluate (c)](#apidoc.element.xpath.XString.prototype.evaluate)
- description and source-code
```javascript
evaluate = function (c) {
	return this;
}
```
- example usage
```shell
...

Using the same interface you have on modern browsers ([MDN])

'''''javascript
var node = null;
var xml = "<book author='J. K. Rowling'><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var result = xpath.evaluate(
    "/book/title",            // xpathExpression
    doc,                        // contextNode
    null,                       // namespaceResolver
    xpath.XPathResult.ANY_TYPE, // resultType
    null                        // result
)
...
```

#### <a name="apidoc.element.xpath.XString.prototype.greaterthan"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>greaterthan (r)](#apidoc.element.xpath.XString.prototype.greaterthan)
- description and source-code
```javascript
greaterthan = function (r) {
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this.number(), Operators.lessthanorequal);
	}
	return this.number().greaterthan(r.number());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString.prototype.greaterthanorequal"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>greaterthanorequal (r)](#apidoc.element.xpath.XString.prototype.greaterthanorequal)
- description and source-code
```javascript
greaterthanorequal = function (r) {
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this.number(), Operators.lessthan);
	}
	return this.number().greaterthanorequal(r.number());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString.prototype.init"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>init (s)](#apidoc.element.xpath.XString.prototype.init)
- description and source-code
```javascript
init = function (s) {
	this.str = String(s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString.prototype.lessthan"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>lessthan (r)](#apidoc.element.xpath.XString.prototype.lessthan)
- description and source-code
```javascript
lessthan = function (r) {
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this.number(), Operators.greaterthanorequal);
	}
	return this.number().lessthan(r.number());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString.prototype.lessthanorequal"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>lessthanorequal (r)](#apidoc.element.xpath.XString.prototype.lessthanorequal)
- description and source-code
```javascript
lessthanorequal = function (r) {
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithNumber(this.number(), Operators.greaterthan);
	}
	return this.number().lessthanorequal(r.number());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString.prototype.nodeset"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>nodeset ()](#apidoc.element.xpath.XString.prototype.nodeset)
- description and source-code
```javascript
nodeset = function () {
	throw new Error("Cannot convert string to nodeset");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString.prototype.notequal"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>notequal (r)](#apidoc.element.xpath.XString.prototype.notequal)
- description and source-code
```javascript
notequal = function (r) {
	if (Utilities.instance_of(r, XBoolean)) {
		return this.bool().notequal(r);
	}
	if (Utilities.instance_of(r, XNumber)) {
		return this.number().notequal(r);
	}
	if (Utilities.instance_of(r, XNodeSet)) {
		return r.compareWithString(this, Operators.notequal);
	}
	return new XBoolean(this.str != r.str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString.prototype.number"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>number ()](#apidoc.element.xpath.XString.prototype.number)
- description and source-code
```javascript
number = function () {
	return new XNumber(this.str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString.prototype.numberValue"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>numberValue ()](#apidoc.element.xpath.XString.prototype.numberValue)
- description and source-code
```javascript
numberValue = function () {
	return this.number().numberValue();
}
```
- example usage
```shell
...
    return function (context, value) {
        assert.equal(2, arguments.length);
        var str = value.stringValue();
        return str + str;
    };
case "square":
    return function (context, value) {
        var num = value.numberValue();
        return num * num;
    };

case "xor":
    return function (context, l, r) {
        assert.equal(3, arguments.length);
        var lbool = l.booleanValue();
...
```

#### <a name="apidoc.element.xpath.XString.prototype.string"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>string ()](#apidoc.element.xpath.XString.prototype.string)
- description and source-code
```javascript
string = function () {
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xpath.XString.prototype.stringValue"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>stringValue ()](#apidoc.element.xpath.XString.prototype.stringValue)
- description and source-code
```javascript
stringValue = function () {
	return this.str;
}
```
- example usage
```shell
...
		var xml = '<book><title>Harry Potter</title></book>';
var doc = new dom().parseFromString(xml);

var parsed = xpath.parse('concat(double(/*/title), " is cool")');

function doubleString(context, value) {
    assert.equal(2, arguments.length);
    var str = value.stringValue();
    return str + str;
}

function functions(name, namespace) {
    if(name === 'double') {
        return doubleString;
    }
...
```

#### <a name="apidoc.element.xpath.XString.prototype.toString"></a>[function <span class="apidocSignatureSpan">xpath.XString.prototype.</span>toString ()](#apidoc.element.xpath.XString.prototype.toString)
- description and source-code
```javascript
toString = function () {
	return this.str;
}
```
- example usage
```shell
...
  , dom = require('xmldom').DOMParser

var xml = "<book><title>Harry Potter</title></book>"
var doc = new dom().parseFromString(xml)
var nodes = xpath.select("//title", doc)

console.log(nodes[0].localName + ": " + nodes[0].firstChild.data)
console.log("Node: " + nodes[0].toString())
'''''
➡

    title: Harry Potter
    Node: <title>Harry Potter</title>

### Alternatively
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
