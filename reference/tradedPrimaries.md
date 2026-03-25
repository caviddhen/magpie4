# tradedPrimaries

Converts trade flows into primary product equivalents by tracing
secondary and livestock products back to their primary inputs. Trade
flows are decomposed into three pathways: (1) direct primary trade, (2)
primaries embodied in secondary products, and (3) primaries needed as
feed for livestock.

## Usage

``` r
tradedPrimaries(gdx, file = NULL)
```

## Arguments

- gdx:

  GDX file

- file:

  a file name the output should be written to using write.magpie

## Value

MAgPIE object with primary product trade equivalents in dry matter (tDM)

## Details

Processing shares and livestock feed baskets of the importing region are
used to calculate primary product requirements. This means that no
footprint can be assigned to secondaries or livestock products
originating from the producer region's processing pathways or feed
baskets. With a bilateral trade implementation, these differences
between producer and importer could be tracked.

## See also

[`land`](land.md), [`croparea`](croparea.md), [`trade`](trade.md)

## Author

Kristine Karstens, David M Chen

## Examples

``` r
if (FALSE) { # \dontrun{
  x <- tradedPrimaries(gdx)
} # }
```
