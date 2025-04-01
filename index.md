<script type='text/javascript'>
	function initEmbeddedMessaging() {
		console.log('Initializing Embedded Messaging...'); // Log when the function starts

		try {
			console.log('Setting language for embedded service:', 'en_US');
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			console.log('Initializing embedded service with parameters:', {
				orgId: '00D5j00000DCDP7',
				siteName: 'Sonim',
				siteURL: 'https://shubhamdeveloper-dev-ed.develop.my.site.com/ESWSonim1743513113880',
				scrt2URL: 'https://shubhamdeveloper-dev-ed.develop.my.salesforce-scrt.com'
			});

			embeddedservice_bootstrap.init(
				'00D5j00000DCDP7',
				'Sonim',
				'https://shubhamdeveloper-dev-ed.develop.my.site.com/ESWSonim1743513113880',
				{
					scrt2URL: 'https://shubhamdeveloper-dev-ed.develop.my.salesforce-scrt.com'
				}
			);

			console.log('Embedded Messaging initialized successfully.');
		} catch (err) {
			console.error('Error loading Embedded Messaging:', err);
		}
	};
</script>
<script type='text/javascript' src='https://shubhamdeveloper-dev-ed.develop.my.site.com/ESWSonim1743513113880/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
