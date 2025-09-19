# To Generate self tickets
# Prechecks and conditions to execute the query
1. A shift count should not greater than 1
2. B shift count should not greater than 2
3. C shift count should not greater than 1
4. G shift count should not greater than 2
5. F shift count should not greater than 2

Note: If F count >2 refer below combination from the bric and use the appropriate one

# Brics to Build F shift

```
when count_f = '3' and rajani = 'F' and vinoth = 'F' and prashant = 'F' and code = 'F1' then 'Rajani'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and prashant = 'F' and code = 'F2' then 'Vinoth'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and prashant = 'F' and code = 'F4' then 'Prashanth'

when count_f = '3' and rajani = 'F' and vinoth = 'F' and kalyan = 'F' and code = 'F1' then 'Rajani'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and kalyan = 'F' and code = 'F2' then 'Vinoth'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and kalyan = 'F' and code = 'F4' then 'Kalyan'

when count_f = '3' and rajani = 'F' and vinoth = 'F' and vineeth = 'F' and code = 'F1' then 'Rajani'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and vineeth = 'F' and code = 'F2' then 'Vinoth'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and vineeth = 'F' and code = 'F4' then 'Vineeth'

when count_f = '3' and rajani = 'F' and vinoth = 'F' and venkadesh = 'F' and code = 'F1' then 'Rajani'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and venkadesh = 'F' and code = 'F2' then 'Vinoth'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and venkadesh = 'F' and code = 'F4' then 'Venkadesh'

when count_f = '3' and rajani = 'F' and vinoth = 'F' and balaji = 'F' and code = 'F1' then 'Rajani'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and balaji = 'F' and code = 'F2' then 'Vinoth'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and balaji = 'F' and code = 'F4' then 'Balaji'

when count_f = '3' and rajani = 'F' and vinoth = 'F' and prakash = 'F' and code = 'F1' then 'Rajani'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and prakash = 'F' and code = 'F2' then 'Vinoth'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and prakash = 'F' and code = 'F4' then 'Prakash'

when count_f = '3' and rajani = 'F' and vinoth = 'F' and prasath = 'F' and code = 'F1' then 'Rajani'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and prasath = 'F' and code = 'F2' then 'Vinoth'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and prasath = 'F' and code = 'F4' then 'Prasath'

```

```
select healthcheck,types,mins,date,
case
when vineeth = 'A'  and shift = 'A' then 'Vineeth'
End as author
from final
where vineeth = 'A' and shift = 'A'

union
select healthcheck,types,mins,date,
case
when prashant = 'A' and shift = 'A' then 'Prashant'
End as author
from final
where prashant = 'A' and shift = 'A'

union
select healthcheck,types,mins,date,
case
when prakash = 'A' and  shift = 'A' then 'Prakash'
End as author
from final
where prakash = 'A' and shift = 'A'

union
select healthcheck,types,mins,date,
case
when balaji = 'A' and shift = 'A' then 'Balaji'
End as author
from final
where balaji = 'A' and shift = 'A'
union
select healthcheck,types,mins,date,
case
when prasath = 'A' and shift = 'A' then 'Prasath'
End as author
from final
where prasath = 'A' and shift = 'A'

union
select healthcheck,types,mins,date,
case
when venkadesh = 'A' and shift = 'A' then 'Venkadesh'
End as author
from final
where venkadesh = 'A' and shift = 'A'

union
select healthcheck,types,mins,date,
case
when kalyan = 'A'  and shift = 'A' then 'Kalyan'
End as author
from final
where kalyan = 'A' and shift = 'A'

union
select healthcheck,types,mins,date,
case
when vineeth = 'C'  and code = 'C' then 'Vineeth'
End as author
from final
where vineeth = 'C' and code = 'C'

union
select healthcheck,types,mins,date,
case
when prashant = 'C' and code = 'C' then 'Prashant'
End as author
from final
where prashant = 'C' and code = 'C'

union
select healthcheck,types,mins,date,
case
when prakash = 'C' and code = 'C' then 'Prakash'
End as author
from final
where prakash = 'C' and code = 'C'

union
select healthcheck,types,mins,date,
case
when balaji = 'C' and code = 'C' then 'Balaji'
End as author
from final
where balaji = 'C' and code = 'C'

union
select healthcheck,types,mins,date,
case
when prasath = 'C' and code = 'C' then 'Prasath'
End as author
from final
where prasath = 'C' and code = 'C'

union
select healthcheck,types,mins,date,
case
when venkadesh = 'C' and code = 'C' then 'Venkadesh'
End as author
from final
where venkadesh = 'C' and code = 'C'

union
select healthcheck,types,mins,date,
case
when kalyan = 'C' and code = 'C' then 'Kalyan'
End as author
from final
where kalyan = 'C' and code = 'C'

union
select healthcheck,types,mins,date,
case

when count_b = '2' and prashant = 'B' and prasath = 'B' and code = 'B1' then 'Prashanth'
when count_b = '2' and prashant = 'B' and prasath = 'B' and code = 'B2' then 'Prasath'

when count_b = '2' and prashant = 'B' and kalyan = 'B' and code = 'B1' then 'Prashanth'
when count_b = '2' and prashant = 'B' and kalyan = 'B' and code = 'B2' then 'Kalyan'

when count_b = '2' and prashant = 'B' and venkadesh = 'B' and code = 'B1' then 'Prashanth'
when count_b = '2' and prashant = 'B' and venkadesh = 'B' and code = 'B2' then 'Venkadesh'

when count_b = '2' and prashant = 'B' and vineeth = 'B' and code = 'B1' then 'Prashanth'
when count_b = '2' and prashant = 'B' and vineeth = 'B' and code = 'B2' then 'Vineeth'

when count_b = '2' and prashant = 'B' and balaji = 'B' and code = 'B1' then 'Prashanth'
when count_b = '2' and prashant = 'B' and balaji = 'B' and code = 'B2' then 'Balaji'

when count_b = '2' and prashant = 'B' and prakash = 'B' and code = 'B1' then 'Prashanth'
when count_b = '2' and prashant = 'B' and prakash = 'B' and code = 'B2' then 'Prakash'

when count_b = '2' and prakash = 'B' and prasath = 'B' and code = 'B1' then 'Prakash'
when count_b = '2' and prakash = 'B' and prasath = 'B' and code = 'B2' then 'Prasath'

when count_b = '2' and prakash = 'B' and kalyan = 'B' and code = 'B1' then 'Prakash'
when count_b = '2' and prakash = 'B' and kalyan = 'B' and code = 'B2' then 'Kalyan'


when count_b = '2' and prakash = 'B' and venkadesh = 'B' and code = 'B1' then 'Prakash'
when count_b = '2' and prakash = 'B' and venkadesh = 'B' and code = 'B2' then 'Venkadesh'

when count_b = '2' and prakash = 'B' and vineeth = 'B' and code = 'B1' then 'Prakash'
when count_b = '2' and prakash = 'B' and vineeth = 'B' and code = 'B2' then 'Vineeth'


when count_b = '2' and prakash = 'B' and balaji = 'B' and code = 'B1' then 'Prakash'
when count_b = '2' and prakash = 'B' and balaji = 'B' and code = 'B2' then 'Balaji'

when count_b = '2' and prasath = 'B' and kalyan = 'B' and code = 'B1' then 'Prasath'
when count_b = '2' and prasath = 'B' and kalyan = 'B' and code = 'B2' then 'Kalyan'

when count_b = '2' and prasath = 'B' and venkadesh = 'B' and code = 'B1' then 'Prasath'
when count_b = '2' and prasath = 'B' and venkadesh = 'B' and code = 'B2' then 'Venkadesh'

when count_b = '2' and prasath = 'B' and vineeth = 'B' and code = 'B1' then 'Prasath'
when count_b = '2' and prasath = 'B' and vineeth = 'B' and code = 'B2' then 'Vineeth'


when count_b = '2' and prasath = 'B' and balaji = 'B' and code = 'B1' then 'Prasath'
when count_b = '2' and prasath = 'B' and balaji = 'B' and code = 'B2' then 'Balaji'

when count_b = '2' and balaji = 'B' and kalyan = 'B' and code = 'B1' then 'Balaji'
when count_b = '2' and balaji = 'B' and kalyan = 'B' and code = 'B2' then 'Kalyan'

when count_b = '2' and balaji = 'B' and venkadesh = 'B' and code = 'B1' then 'Balaji'
when count_b = '2' and balaji = 'B' and venkadesh = 'B' and code = 'B2' then 'Venkadesh'


when count_b = '2' and balaji = 'B' and vineeth = 'B' and code = 'B1' then 'Balaji'
when count_b = '2' and balaji = 'B' and vineeth = 'B' and code = 'B2' then 'Vineeth'

when count_b = '2' and kalyan = 'B' and venkadesh = 'B' and code = 'B1' then 'Kalyan'
when count_b = '2' and kalyan = 'B' and venkadesh = 'B' and code = 'B2' then 'Venkadesh'

when count_b = '2' and kalyan = 'B' and vineeth = 'B' and code = 'B1' then 'Kalyan'
when count_b = '2' and kalyan = 'B' and vineeth = 'B' and code = 'B2' then 'Vineeth'


when count_b = '2' and venkadesh = 'B' and vineeth = 'B' and code = 'B1' then 'Venkadesh'
when count_b = '2' and venkadesh = 'B' and vineeth = 'B' and code = 'B2' then 'Vineeth'

when count_b = '2' and vinoth = 'B' and prashant = 'B' and code = 'B1' then 'Vinoth'
when count_b = '2' and vinoth = 'B' and prashant = 'B' and code = 'B2' then 'Prashanth'


when count_b = '2' and vinoth = 'B' and prakash = 'B' and code = 'B1' then 'Vinoth'
when count_b = '2' and vinoth = 'B' and prakash = 'B' and code = 'B2' then 'Prakash'


when count_b = '2' and vinoth = 'B' and kalyan = 'B' and code = 'B1' then 'Vinoth'
when count_b = '2' and vinoth = 'B' and kalyan = 'B' and code = 'B2' then 'Kalyan' 


when count_b = '2' and vinoth = 'B' and balaji = 'B' and code = 'B1' then 'Vinoth'
when count_b = '2' and vinoth = 'B' and balaji = 'B' and code = 'B2' then 'Balaji'

when count_b = '2' and vinoth = 'B' and venkadesh = 'B' and code = 'B1' then 'Vinoth'
when count_b = '2' and vinoth = 'B' and venkadesh = 'B' and code = 'B2' then 'Venkadesh'

when count_b = '2' and vinoth = 'B' and vineeth = 'B' and code = 'B1' then 'Vinoth'
when count_b = '2' and vinoth = 'B' and vineeth = 'B' and code = 'B2' then 'Vineeth'

when count_b = '2' and vinoth = 'B' and prasath = 'B'  and code = 'B1' then 'Vinoth'
when count_b = '2' and vinoth = 'B' and prasath = 'B'  and code = 'B2' then 'Prasath'

when count_b = '1' and vineeth = 'B' and shift = 'B' then 'Vineeth'
when count_b = '1' and prakash = 'B' and shift = 'B' then 'Prakash'
when count_b = '1' and balaji = 'B' and shift = 'B' then 'Balaji'
when count_b = '1' and prashant = 'B' and shift = 'B' then 'Prashanth'
when count_b = '1' and venkadesh = 'B' and shift = 'B' then 'Venkadesh'
when count_b = '1' and prasath = 'B' and shift = 'B' then 'Prasath'
when count_b = '1' and kalyan = 'B' and shift = 'B' then 'Kalyan'
when count_b = '1' and vinoth = 'B' and shift = 'B' then 'Vinoth'
end as author
from final
where shift = 'B'

union

select healthcheck,types,mins,date,
case

when count_g = '2' and prashant = 'G' and prasath = 'G' and code = 'G1' then 'Prashanth'
when count_g = '2' and prashant = 'G' and prasath = 'G' and code = 'G2' then 'Prasath'

when count_g = '2' and prashant = 'G' and kalyan = 'G' and code = 'G1' then 'Prashanth'
when count_g = '2' and prashant = 'G' and kalyan = 'G' and code = 'G2' then 'Kalyan'

when count_g = '2' and prashant = 'G' and venkadesh = 'G' and code = 'G1' then 'Prashanth'
when count_g = '2' and prashant = 'G' and venkadesh = 'G' and code = 'G2' then 'Venkadesh'

when count_g = '2' and prashant = 'G' and vineeth = 'G' and code = 'G1' then 'Prashanth'
when count_g = '2' and prashant = 'G' and vineeth = 'G' and code = 'G2' then 'Vineeth'

when count_g = '2' and prashant = 'G' and balaji = 'G' and code = 'G1' then 'Prashanth'
when count_g = '2' and prashant = 'G' and balaji = 'G' and code = 'G2' then 'balaji'

when count_g = '2' and prashant = 'G' and prakash = 'G' and code = 'G1' then 'Prashanth'
when count_g = '2' and prashant = 'G' and prakash = 'G' and code = 'G2' then 'Prakash'

when count_g = '2' and prakash = 'G' and prasath = 'G' and code = 'G1' then 'Prakash'
when count_g = '2' and prakash = 'G' and prasath = 'G' and code = 'G2' then 'Prasath'

when count_g = '2' and prakash = 'G' and kalyan = 'G' and code = 'G1' then 'Prakash'
when count_g = '2' and prakash = 'G' and kalyan = 'G' and code = 'G2' then 'Kalyan'


when count_g = '2' and prakash = 'G' and venkadesh = 'G' and code = 'G1' then 'Prakash'
when count_g = '2' and prakash = 'G' and venkadesh = 'G' and code = 'G2' then 'Venkadesh'

when count_g = '2' and prakash = 'G' and vineeth = 'G' and code = 'G1' then 'Prakash'
when count_g = '2' and prakash = 'G' and vineeth = 'G' and code = 'G2' then 'Vineeth'


when count_g = '2' and prakash = 'G' and balaji = 'G' and code = 'G1' then 'Prakash'
when count_g = '2' and prakash = 'G' and balaji = 'G' and code = 'G2' then 'balaji'

when count_g = '2' and prasath = 'G' and kalyan = 'G' and code = 'G1' then 'Prasath'
when count_g = '2' and prasath = 'G' and kalyan = 'G' and code = 'G2' then 'Kalyan'

when count_g = '2' and prasath = 'G' and venkadesh = 'G' and code = 'G1' then 'Prasath'
when count_g = '2' and prasath = 'G' and venkadesh = 'G' and code = 'G2' then 'Venkadesh'

when count_g = '2' and prasath = 'G' and vineeth = 'G' and code = 'G1' then 'Prasath'
when count_g = '2' and prasath = 'G' and vineeth = 'G' and code = 'G2' then 'Vineeth'


when count_g = '2' and prasath = 'G' and balaji = 'G'	and code = 'G1' then 'Prasath'
when count_g = '2' and prasath = 'G' and balaji = 'G'	and code = 'G2' then 'balaji'

when count_g = '2' and balaji = 'G' and kalyan = 'G' and code = 'G1' then 'balaji'
when count_g = '2' and balaji = 'G' and kalyan = 'G' and code = 'G2' then 'Kalyan'

when count_g = '2' and balaji = 'G' and venkadesh = 'G' and code = 'G1' then 'balaji'
when count_g = '2' and balaji = 'G' and venkadesh = 'G' and code = 'G2' then 'Venkadesh'


when count_g = '2' and balaji = 'G' and vineeth = 'G' and code = 'G1' then 'balaji'
when count_g = '2' and balaji = 'G' and vineeth = 'G' and code = 'G2' then 'Vineeth'

when count_g = '2' and kalyan = 'G' and venkadesh = 'G' and code = 'G1' then 'Kalyan'
when count_g = '2' and kalyan = 'G' and venkadesh = 'G' and code = 'G2' then 'Venkadesh'

when count_g = '2' and kalyan = 'G' and vineeth = 'G' and code = 'G1' then 'Kalyan'
when count_g = '2' and kalyan = 'G' and vineeth = 'G' and code = 'G2' then 'Vineeth'


when count_g = '2' and venkadesh = 'G' and vineeth = 'G' and code = 'G1' then 'Venkadesh'
when count_g = '2' and venkadesh = 'G' and vineeth = 'G' and code = 'G2' then 'Vineeth'

when count_g = '2' and vinoth = 'G' and prashant = 'G' and code = 'G1' then 'Vinoth'
when count_g = '2' and vinoth = 'G' and prashant = 'G' and code = 'G2' then 'Prashanth'


when count_g = '2' and vinoth = 'G' and prakash = 'G' and code = 'G1' then 'Vinoth'
when count_g = '2' and vinoth = 'G' and prakash = 'G' and code = 'G2' then 'Prakash'


when count_g = '2' and vinoth = 'G' and kalyan = 'G' and code = 'G1' then 'Vinoth'
when count_g = '2' and vinoth = 'G' and kalyan = 'G' and code = 'G2' then 'Kalyan' 


when count_g = '2' and vinoth = 'G' and balaji = 'G' and code = 'G1' then 'Vinoth'
when count_g = '2' and vinoth = 'G' and balaji = 'G' and code = 'G2' then 'balaji'

when count_g = '2' and vinoth = 'G' and venkadesh = 'G' and code = 'G1' then 'Vinoth'
when count_g = '2' and vinoth = 'G' and venkadesh = 'G' and code = 'G2' then 'Venkadesh'

when count_g = '2' and vinoth = 'G' and vineeth = 'G' and code = 'G1' then 'Vinoth'
when count_g = '2' and vinoth = 'G' and vineeth = 'G' and code = 'G2' then 'Vineeth'

when count_g = '2' and vinoth = 'G' and prasath = 'G'  and code = 'G1' then 'Vinoth'
when count_g = '2' and vinoth = 'G' and prasath = 'G'  and code = 'G2' then 'Prasath'

when count_g = '1' and vineeth = 'G' and shift = 'G' then 'Vineeth'
when count_g = '1' and prakash = 'G' and shift = 'G' then 'Prakash'
when count_g = '1' and balaji = 'G' and shift = 'G' then 'balaji'
when count_g = '1' and prashant = 'G' and shift = 'G' then 'Prashanth'
when count_g = '1' and venkadesh = 'G' and shift = 'G' then 'Venkadesh'
when count_g = '1' and prasath = 'G' and shift = 'G' then 'Prasath'
when count_g = '1' and kalyan = 'G' and shift = 'G' then 'Kalyan'
when count_g = '1' and vinoth = 'G' and shift = 'G' then 'Vinoth'
when count_g = '0' and prakash = 'A' and shift = 'G' then 'Prakash'
when count_g = '0' and prasath = 'A' and shift = 'G' then 'Prasath'
when count_g = '0' and prashant = 'A' and shift = 'G' then 'Prashanth'
when count_g = '0' and vineeth = 'A' and shift = 'G' then 'Vineeth'
when count_g = '0' and kalyan = 'A' and shift = 'G' then 'Kalyan'
when count_g = '0' and venkadesh = 'A' and shift = 'G' then 'Venkadesh'
when count_g = '0' and balaji = 'A' and shift = 'G' then 'Balaji'
when count_g = '0' and vinoth = 'A' and shift = 'G' then 'Vinoth'

end as author
from final
where shift = 'G'

union
select healthcheck,types,mins,date,
case
-- to elect 2 from 9
when count_f = '2' and prashant = 'F' and prasath = 'F' and code1 = 'F4' then 'Prashanth'
when count_f = '2' and prashant = 'F' and prasath = 'F' and code = 'F4' then 'Prasath'

when count_f = '2' and prashant = 'F' and kalyan = 'F' and code1 = 'F4' then 'Prashanth'
when count_f = '2' and prashant = 'F' and kalyan = 'F' and code = 'F4' then 'Kalyan'

when count_f = '2' and prashant = 'F' and venkadesh = 'F' and code1 = 'F4' then 'Prashanth'
when count_f = '2' and prashant = 'F' and venkadesh = 'F' and code = 'F4' then 'Venkadesh'

when count_f = '2' and prashant = 'F' and vineeth = 'F' and code1 = 'F4' then 'Prashanth'
when count_f = '2' and prashant = 'F' and vineeth = 'F' and code = 'F4' then 'Vineeth'

when count_f = '2' and prashant = 'F' and balaji = 'F' and code1 = 'F4' then 'Prashanth'
when count_f = '2' and prashant = 'F' and balaji = 'F' and code = 'F4' then 'balaji'

when count_f = '2' and prashant = 'F' and prakash = 'F' and code1 = 'F4' then 'Prashanth'
when count_f = '2' and prashant = 'F' and prakash = 'F' and code = 'F4' then 'Prakash'

when count_f = '2' and prakash = 'F' and prasath = 'F' and code1 = 'F4' then 'Prakash'
when count_f = '2' and prakash = 'F' and prasath = 'F' and code = 'F4' then 'Prasath'

when count_f = '2' and prakash = 'F' and kalyan = 'F' and code1 = 'F4' then 'Prakash'
when count_f = '2' and prakash = 'F' and kalyan = 'F' and code = 'F4' then 'Kalyan'


when count_f = '2' and prakash = 'F' and venkadesh = 'F' and code1 = 'F4' then 'Prakash'
when count_f = '2' and prakash = 'F' and venkadesh = 'F' and code = 'F4' then 'Venkadesh'

when count_f = '2' and prakash = 'F' and vineeth = 'F' and code1 = 'F4' then 'Prakash'
when count_f = '2' and prakash = 'F' and vineeth = 'F' and code = 'F4' then 'Vineeth'


when count_f = '2' and prakash = 'F' and balaji = 'F' and code1 = 'F4' then 'Prakash'
when count_f = '2' and prakash = 'F' and balaji = 'F' and code = 'F4' then 'balaji'

when count_f = '2' and prasath = 'F' and kalyan = 'F' and code1 = 'F4' then 'Prasath'
when count_f = '2' and prasath = 'F' and kalyan = 'F' and code = 'F4' then 'Kalyan'

when count_f = '2' and prasath = 'F' and venkadesh = 'F' and code1 = 'F4' then 'Prasath'
when count_f = '2' and prasath = 'F' and venkadesh = 'F' and code = 'F4' then 'Venkadesh'

when count_f = '2' and prasath = 'F' and vineeth = 'F' and code1 = 'F4' then 'Prasath'
when count_f = '2' and prasath = 'F' and vineeth = 'F' and code = 'F4' then 'Vineeth'


when count_f = '2' and prasath = 'F' and balaji = 'F' and code1 = 'F4' then 'Prasath'
when count_f = '2' and prasath = 'F' and balaji = 'F' and code = 'F4' then 'balaji'

when count_f = '2' and balaji = 'F' and kalyan = 'F' and code1 = 'F4' then 'balaji'
when count_f = '2' and balaji = 'F' and kalyan = 'F' and code = 'F4' then 'Kalyan'

when count_f = '2' and balaji = 'F' and venkadesh = 'F' and code1 = 'F4' then 'balaji'
when count_f = '2' and balaji = 'F' and venkadesh = 'F' and code = 'F4' and code = 'F4' then 'Venkadesh'


when count_f = '2' and balaji = 'F' and vineeth = 'F' and code1 = 'F4' then 'balaji'
when count_f = '2' and balaji = 'F' and vineeth = 'F' and code = 'F4' then 'Vineeth'

when count_f = '2' and kalyan = 'F' and venkadesh = 'F' and code1 = 'F4' then 'Kalyan'
when count_f = '2' and kalyan = 'F' and venkadesh = 'F' and code = 'F4' then 'Venkadesh'

when count_f = '2' and kalyan = 'F' and vineeth = 'F' and code1 = 'F4' then 'Kalyan'
when count_f = '2' and kalyan = 'F' and vineeth = 'F' and code = 'F4' then 'Vineeth'


when count_f = '2' and venkadesh = 'F' and vineeth = 'F' and code1 = 'F4' then 'Venkadesh'
when count_f = '2' and venkadesh = 'F' and vineeth = 'F' and code = 'F4' then 'Vineeth'

when count_f = '2' and vinoth = 'F' and prashant = 'F' and code1 = 'F4' then 'Vinoth'
when count_f = '2' and vinoth = 'F' and prashant = 'F' and code = 'F4' then 'Prashanth'


when count_f = '2' and vinoth = 'F' and prakash = 'F' and code1 = 'F4' then 'Vinoth'
when count_f = '2' and vinoth = 'F' and prakash = 'F' and code = 'F4' then 'Prakash'


when count_f = '2' and vinoth = 'F' and kalyan = 'F' and code1 = 'F4' then 'Vinoth'
when count_f = '2' and vinoth = 'F' and kalyan = 'F' and code = 'F4' then 'Kalyan' 


when count_f = '2' and vinoth = 'F' and balaji = 'F' and code1 = 'F4' then 'Vinoth'
when count_f = '2' and vinoth = 'F' and balaji = 'F' and code = 'F4' then 'balaji'

when count_f = '2' and vinoth = 'F' and venkadesh = 'F' and code1 = 'F4' then 'Vinoth'
when count_f = '2' and vinoth = 'F' and venkadesh = 'F' and code = 'F4' then 'Venkadesh'

when count_f = '2' and vinoth = 'F' and vineeth = 'F' and code1 = 'F4' then 'Vinoth'
when count_f = '2' and vinoth = 'F' and vineeth = 'F' and code = 'F4' then 'Vineeth'

when count_f = '2' and vinoth = 'F' and prasath = 'F'  and code1 = 'F4' then 'Vinoth'
when count_f = '2' and vinoth = 'F' and prasath = 'F'  and code = 'F4' then 'Prasath'

when count_f = '2' and rajani = 'F' and prakash = 'F' and code1 = 'F4' then 'Rajani'
when count_f = '2' and rajani = 'F' and prakash = 'F' and code = 'F4' then 'Prakash'


when count_f = '2' and rajani = 'F' and prashant = 'F' and code1 = 'F4' then 'Rajani'
when count_f = '2' and rajani = 'F' and prashant = 'F' and code = 'F4' then 'Prashanth'

when count_f = '2' and rajani = 'F' and vineeth = 'F' and code1 = 'F4' then 'Rajani'
when count_f = '2' and rajani = 'F' and vineeth = 'F' and code = 'F4' then 'Vineeth'


when count_f = '2' and rajani = 'F' and vinoth = 'F' and code1 = 'F4' then 'Rajani'
when count_f = '2' and rajani = 'F' and vinoth = 'F' and code = 'F4' then 'Vinoth'


when count_f = '2' and rajani = 'F' and balaji = 'F' and code1 = 'F4' then 'Rajani'
when count_f = '2' and rajani = 'F' and balaji = 'F' and code = 'F4' then 'Balaji'


when count_f = '2' and rajani = 'F' and venkadesh = 'F' and code1 = 'F4' then 'Rajani'
when count_f = '2' and rajani = 'F' and venkadesh = 'F' and code = 'F4' then 'Venkadesh'


when count_f = '2' and rajani = 'F' and kalyan = 'F' and code1 = 'F4' then 'Rajani'
when count_f = '2' and rajani = 'F' and kalyan = 'F' and code = 'F4' then 'Kalyan'


when count_f = '2' and rajani = 'F' and prasath = 'F' and code1 = 'F4' then 'Rajani'
when count_f = '2' and rajani = 'F' and prasath = 'F' and code = 'F4' then 'Prasath'

when count_f = '1' and rajani = 'F' and shift = 'F' then 'Rajani'
when count_f = '1' and vineeth = 'F' and shift = 'F' then 'Vineeth'
when count_f = '1' and prakash = 'F' and shift = 'F' then 'Prakash'
when count_f = '1' and balaji = 'F' and shift = 'F' then 'balaji'
when count_f = '1' and prashant = 'F' and shift = 'F' then 'Prashanth'
when count_f = '1' and venkadesh = 'F' and shift = 'F' then 'Venkadesh'
when count_f = '1' and prasath = 'F' and shift = 'F' then 'Prasath'
when count_f = '1' and kalyan = 'F' and shift = 'F' then 'Kalyan'
when count_f = '1' and vinoth = 'F' and shift = 'F' then 'Vinoth'
when count_f = '0' and prakash = 'A' and shift = 'F' then 'Prakash'
when count_f = '0' and prasath = 'A' and shift = 'F' then 'Prasath'
when count_f = '0' and prashant = 'A' and shift = 'F' then 'Prashanth'
when count_f = '0' and vineeth = 'A' and shift = 'F' then 'Vineeth'
when count_f = '0' and kalyan = 'A' and shift = 'F' then 'Kalyan'
when count_f = '0' and venkadesh = 'A' and shift = 'F' then 'Venkadesh'
when count_f = '0' and balaji = 'A' and shift = 'F' then 'Balaji'
when count_f = '0' and vinoth = 'A' and shift = 'F' then 'Vinoth'

when count_f = '3' and rajani = 'F' and vinoth = 'F' and prakash = 'F' and code = 'F1' then 'Rajani'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and prakash = 'F' and code = 'F2' then 'Vinoth'
when count_f = '3' and rajani = 'F' and vinoth = 'F' and prakash = 'F' and code = 'F4' then 'Prakash'

end as author
from final
where shift = 'F'

union
select healthcheck,types,mins,date,
case
when vinoth != 'W.OFF' and shift = 'E' then 'Vinoth'
when vinoth = 'W.OFF' and vineeth = 'A' and shift = 'E' then 'Vineeth'
when vinoth = 'W.OFF' and prakash = 'A' and shift = 'E' then 'Prakash'
when vinoth = 'W.OFF' and kalyan = 'A' and shift = 'E' then 'Kalyan'
when vinoth = 'W.OFF' and balaji = 'A' and shift = 'E' then 'Balaji'
when vinoth = 'W.OFF' and venkadesh = 'A' and shift = 'E' then 'Venkadesh'
when vinoth = 'W.OFF' and prasath = 'A' and shift = 'E' then 'Prasath' 
when vinoth = 'W.OFF' and prashant = 'A' and shift = 'E' then 'Prashanth' 

end as author
from final
where shift = 'E' 

```
