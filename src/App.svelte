<svelte:options tag="flapp-account" />

<script>
</script>

<div class="bg-light">
	<div class="container"><br>
		<div class="row">
			<div class="col-md-8 order-md-1">
				<h4 class="mb-3">Account</h4>
				<form class="needs-validation" novalidate>
					<div class="row">
						<div class="col-md-6 mb-3">
							<label for="firstName">First name</label>
							<input type="text" class="form-control" id="firstName" placeholder="" value="Jose" required>
							<div class="invalid-feedback">
								Valid first name is required.
							</div>
						</div>
						<div class="col-md-6 mb-3">
							<label for="lastName">Last name</label>
							<input type="text" class="form-control" id="lastName" placeholder="" value="Navarro" required>
							<div class="invalid-feedback">
								Valid last name is required.
							</div>
						</div>
					</div>

					<div class="mb-3">
						<label for="username">Username</label>
						<div class="input-group">
							<div class="input-group-prepend">
								<span class="input-group-text">@</span>
							</div>
							<input type="text" class="form-control" id="username" placeholder="Username" value="netflapp" required>
							<div class="invalid-feedback" style="width: 100%;">
								Your username is required.
							</div>
						</div>
					</div>

					<div class="mb-3">
						<label for="email">Email <span class="text-muted">(Optional)</span></label>
						<input type="email" class="form-control" id="email" value="hola@netflapp.com">
						<div class="invalid-feedback">
							Please enter a valid email address for shipping updates.
						</div>
					</div>

					<div class="mb-3">
						<label for="address">Address</label>
						<input type="text" class="form-control" id="address" value="1234 Main St" required>
						<div class="invalid-feedback">
							Please enter your shipping address.
						</div>
					</div>

					<div class="row">
						<div class="col-md-5 mb-3">
							<label for="country">Country</label>
							<select class="custom-select d-block w-100" id="country" required>
								<option value="">Choose...</option>
								<option selected>Colombia</option>
							</select>
							<div class="invalid-feedback">
								Please select a valid country.
							</div>
						</div>
						<div class="col-md-4 mb-3">
							<label for="state">State</label>
							<select class="custom-select d-block w-100" id="state" required>
								<option value="">Choose...</option>
								<option selected>Barranquilla</option>
							</select>
							<div class="invalid-feedback">
								Please provide a valid state.
							</div>
						</div>
						<div class="col-md-3 mb-3">
							<label for="zip">Zip</label>
							<input type="text" class="form-control" id="zip" placeholder="" value="00000" required>
							<div class="invalid-feedback">
								Zip code required.
							</div>
						</div>
					</div>
					<hr class="mb-4">

					<h4 class="mb-3">Payment</h4>

					<div class="d-block my-3">
						<div class="custom-control custom-radio">
							<input id="credit" name="paymentMethod" type="radio" class="custom-control-input" checked required>
							<label class="custom-control-label" for="credit">Credit card</label>
						</div>
						<div class="custom-control custom-radio">
							<input id="debit" name="paymentMethod" type="radio" class="custom-control-input" required>
							<label class="custom-control-label" for="debit">Debit card</label>
						</div>
						<div class="custom-control custom-radio">
							<input id="paypal" name="paymentMethod" type="radio" class="custom-control-input" required>
							<label class="custom-control-label" for="paypal">PayPal</label>
						</div>
					</div>
					<div class="row">
						<div class="col-md-6 mb-3">
							<label for="cc-name">Name on card</label>
							<input type="text" class="form-control" id="cc-name" value="Example ..." required>
							<small class="text-muted">Full name as displayed on card</small>
							<div class="invalid-feedback">
								Name on card is required
							</div>
						</div>
						<div class="col-md-6 mb-3">
							<label for="cc-number">Credit card number</label>
							<input type="text" class="form-control" id="cc-number" placeholder="" value="4111 1111 1111 1111" required>
							<div class="invalid-feedback">
								Credit card number is required
							</div>
						</div>
					</div>
					<div class="row">
						<div class="col-md-3 mb-3">
							<label for="cc-expiration">Expiration</label>
							<input type="text" class="form-control" id="cc-expiration" placeholder="" value="11 / 2022" required>
							<div class="invalid-feedback">
								Expiration date required
							</div>
						</div>
						<div class="col-md-3 mb-3">
							<label for="cc-cvv">CVV</label>
							<input type="text" class="form-control" id="cc-cvv" placeholder="" value="111" required>
							<div class="invalid-feedback">
								Security code required
							</div>
						</div>
					</div>
					<hr class="mb-4">
					<button class="btn btn-primary btn-lg btn-block" type="submit">Guardar.</button>
				</form>
			</div>
		</div>
	</div>
</div>
<style>
	@import "https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css";

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
