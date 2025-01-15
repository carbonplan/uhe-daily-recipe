\
## Questions:
How do we extract commit message? It would be nice to store dates/indexes here
icechunk.xarray.to_icechunk(ds, store=store,region="auto", consoldated=False, zarr_format=3) region doesn't seem to work?
We should open up a MRE...



### hmm okay so append_dim returns the distributed commits 'works', but data doesn't exists
# region doesn't work... is this a bug?
# seems like we have to use the icechunk.to_zarr
# next up.. can we just insert with Zarr or at a specific time slice with region..
# then we batch, write, commit?
# or do it all and commits are tagged?
