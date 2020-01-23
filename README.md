# RowEchelonGenField.jl
A naive implementation of row reduced echelon form of a matrix over a general field.

Since the RowEchelon package was removed from base because of it not being general and converting
everything to floats, i made this for my own convenience when doing linear algebra over different fields.
By field i mean any type that implements addition, mutiplication, division and a one and zero function.
If the type implements those but is not a field (quaternions or integers mod a composite number for example)
i have no guarantee of the behaviour.

I will mostly have the inbuilt Rational type in mind when making this, but it should work for any other field
such as Integers mod primes, Floats (although rounding funkyness is not though about (hence naive)) and most
other types behaving as a field.
