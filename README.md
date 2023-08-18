# Pirichain-api-python

Package for Pirichain API calls through Python
============
![PyPI - Downloads](https://img.shields.io/pypi/dw/pirichain-api-workmail20)    ![PyPI - License](https://img.shields.io/pypi/l/pirichain-api-workmail20)    ![PyPI - Format](https://img.shields.io/pypi/format/pirichain-api-workmail20)    ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pirichain-api-workmail20)    ![PyPI](https://img.shields.io/pypi/v/pirichain-api-workmail20)



---
Pirichain is blockchain system that based on dPos (Delegated Proof of Stake) and has it own environment to create wallet and token, transactions, sending or storing data as a transaction, delegation.


Requirements
------------

* Python >= 3.7;

Installation
------------

    pip install pirichain-api-workmail20


Usage
------------
```python
from workmail20.pirichain import PIRIAPI_w20

piri = PIRIAPI_w20(True)

print(piri.createNewAddress())
print(piri.createNewAddress("portuguese",True))
print(piri.rescuePrivateKey("entry frequent airport firm document close human roof fix pond popular laugh banner fruit faint exact sleep axis pipe crush today elder inform saddle"))
print(piri.getMnemonic("4bab94162ba406575bb5dd5814faa0bec124bb947a72cb221e951a8e348e9ce5"))
print(piri.getBalance("PRTMRWG479eCmbbufg92qZsysYHMH7bRL7H6eDVwNSx"))
print(piri.getBalanceList("PRTMRgoFporAfQYrNNJfj3Go37FT5AR3ueKCwpdKd1s"))
print(piri.getToken())
print(piri.listTokens())
print(piri.getScenario("PRTMQ7fcZp7ACGDEom4KJQ4bvJ5nwQ3CcaUTFy642mE"))
print(piri.listMyScenarios("PRTMPUAV2mTGq6Dpu9ZBYmJyXWdt9RYiiouvRaZ8xUR"))
print(piri.listScenarios())
print(piri.executeScenario("PRTMPBjj3sutTtHwvRgB8YFHtMdcTv1Bd7cMWMxMrZP","PRTMRWG479eCmbbufg92qZsysYHMH7bRL7H6eDVwNSx",
"9d656610ec7ff8a8e7e9225234ee54b6fa31d147981e1b91106ce901ae69bf00","init",'["11","22","333"]'))
print(piri.previewScenario("{}","PRTMRWG479eCmbbufg92qZsysYHMH7bRL7H6eDVwNSx",
"9d656610ec7ff8a8e7e9225234ee54b6fa31d147981e1b91106ce901ae69bf00","init",'["11","22","333"]'))
print(piri.listTransactions())
print(piri.listPoolTransactions())
print(piri.listTransactionsByAssetID("-1","0","50"))
print(piri.listTransactionsByAddr("PRTMPUAV2mTGq6Dpu9ZBYmJyXWdt9RYiiouvRaZ8xUR","0","50"))
print(piri.getTransaction("f0f5733c7cc71ad3ae2dea4417c7e16a39aed9edba6a4c414568875b30a1ad9b"))
print(piri.getPoolTransaction("f0f5733c7cc71ad3ae2dea4417c7e16a39aed9edba6a4c414568875b30a1ad9b"))
print(piri.getBlocks())
print(piri.getBlocksDesc())
print(piri.getLastBlocks())
print(piri.getOnlyBlocks())
print(piri.getBlock("2673310"))
print(piri.pushData("PRTMRWG479eCmbbufg92qZsysYHMH7bRL7H6eDVwNSx","9d656610ec7ff8a8e7e9225234ee54b6fa31d147981e1b91106ce901ae69bf00","PRTMRN71Mz5mrZMA59mPtURrTG9S4yydYDyi1YNi5uX",
'{"key":"xxxx1","value":"000","enc":0}',
"043e6ace02e5b6c8031455d91ae88b411b80935f48404c6014075043e71d2ffb8da3b2f5f3a480f9be45b9455b846781bdbdf6466076645cc86e5a00c82c51bc00"))
print(piri.pushDataList("PRTMRWG479eCmbbufg92qZsysYHMH7bRL7H6eDVwNSx","9d656610ec7ff8a8e7e9225234ee54b6fa31d147981e1b91106ce901ae69bf00","PRTMRN71Mz5mrZMA59mPtURrTG9S4yydYDyi1YNi5uX",
'[{"key":"xxxx2","value":"000","enc":0},{"key":"xxxx3","value":"000","enc":0}]'))
print(piri.listData())
print(piri.listDataByAddress("PRTMRN71Mz5mrZMA59mPtURrTG9S4yydYDyi1YNi5uX"))
print(piri.getAddressListByAsset())
print(piri.isValidAddress("PRTMRN71Mz5mrZMA59mPtURrTG9S4yydYDyi1YNi5u0"))
print(piri.search("99f9f4ec7012db95868bb9526cd9b239765634183b64ad3eb7b3c13daf5ed12d"))
print(piri.search("2673310"))
print(apiri.listData())
print(piri.listDeputies())
print(piri.checkDeputy("PRTMPRSg92ndyu5NeaEf7q3D6TdJeKKa6nKStVMcU4e"))
print(piri.getMyRewardQuantity("PRTMRWG479eCmbbufg92qZsysYHMH7bRL7H6eDVwNSx","9d656610ec7ff8a8e7e9225234ee54b6fa31d147981e1b91106ce901ae69bf00"))
print(piri.getPiriPrice())
print(piri.getRichList())
print(piri.getDetailStats())
print(piri.getStats())
print(piri.listDelegationTopN())
print(piri.getCirculation())

```

API documentation
------------

For more detailed and up-to-date API documentation, you can access it at https://api.pirichain.com and refer to the Postman collection documents specified at that address.

Changelog
------------

To keep track, please refer to [CHANGELOG.md](https://github.com/workmail20/pirichain-api-python/blob/master/CHANGELOG.md).