import React from 'react';

// Main App component
const App = () => {
  return (
    <div className="min-h-screen bg-sky-50 font-inter text-gray-800 flex flex-col items-center p-4 sm:p-8">
      {/* Header Section */}
      <header className="w-full max-w-6xl flex flex-col sm:flex-row items-center justify-between py-6 px-4 bg-white rounded-xl shadow-lg mb-8">
        <div className="flex items-center mb-4 sm:mb-0">
          {/* Logo */}
          <img
            src="Tonguy Platforms Logo tgp 2024 smaller (1).png" // Using the smaller logo for better fit
            alt="Tonguy Platforms Logo"
            className="h-16 w-16 sm:h-20 sm:w-20 rounded-full object-cover mr-4"
            onError={(e) => {
              e.target.onerror = null;
              e.target.src = "https://placehold.co/80x80/E0E7FF/4338CA?text=Logo"; // Placeholder if image fails
            }}
          />
          <h1 className="text-3xl sm:text-4xl font-extrabold text-sky-700">Tonguy Platforms</h1>
        </div>
        <p className="text-lg sm:text-xl font-semibold text-gray-600 mt-2 sm:mt-0">Connected Beings.</p>
      </header>

      {/* About Section */}
      <section className="w-full max-w-6xl bg-white rounded-xl shadow-lg p-6 sm:p-8 mb-8 text-center">
        <h2 className="text-2xl sm:text-3xl font-bold text-sky-600 mb-4">About Us</h2>
        <p className="text-base sm:text-lg leading-relaxed text-gray-700">
          Tonguy Platforms is an applications and development company dedicated to enhancing human connectivity
          for business and social interactions. We strive to create innovative technologies that address
          everyday challenges and foster meaningful connections in the digital world.
        </p>
      </section>

      {/* Projects Section */}
      <section className="w-full max-w-6xl bg-white rounded-xl shadow-lg p-6 sm:p-8 mb-8">
        <h2 className="text-2xl sm:text-3xl font-bold text-sky-600 mb-6 text-center">Our Projects</h2>
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          {/* Project Widget: Lost & Found */}
          <ProjectWidget
            title="Lost & Found"
            description="A platform designed to help people easily report and recover lost items, fostering community assistance."
            link="http://www.lost&found.com"
            imageUrl="https://placehold.co/400x250/A78BFA/FFFFFF?text=Lost+%26+Found" // Placeholder image
          />
          {/* Project Widget: DBC - Digital Business Cards */}
          <ProjectWidget
            title="DBC - Digital Business Cards"
            description="Revolutionize networking with eco-friendly and interactive digital business cards."
            link="#" // No external link provided, so using '#'
            imageUrl="https://placehold.co/400x250/60A5FA/FFFFFF?text=Digital+Business+Cards" // Placeholder image
          />
        </div>
      </section>

      {/* Social Media Section */}
      <section className="w-full max-w-6xl bg-white rounded-xl shadow-lg p-6 sm:p-8 mb-8 text-center">
        <h2 className="text-2xl sm:text-3xl font-bold text-sky-600 mb-6">Connect With Us</h2>
        <div className="flex flex-wrap justify-center gap-6">
          <SocialLink
            platform="LinkedIn"
            icon="M20 20h-4v-7.98c0-.98-.02-2.23-1.36-2.23-1.37 0-1.58 1.07-1.58 2.17V20H9V9h3.83v1.65h.05c.53-.98 1.81-1.79 3.76-1.79 4.02 0 4.76 2.64 4.76 6.08V20zM7 6.5C7 5.67 6.33 5 5.5 5S4 5.67 4 6.5 4.67 8 5.5 8 7 7.33 7 6.5z"
            url="https://www.linkedin.com/company/tonguy-platforms"
          />
          <SocialLink
            platform="Instagram"
            icon="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 2c2.76 0 5 2.24 5 5s-2.24 5-5 5-5-2.24-5-5 2.24-5 5-5zm0 1.8c-1.77 0-3.2 1.43-3.2 3.2s1.43 3.2 3.2 3.2 3.2-1.43 3.2-3.2-1.43-3.2-3.2-3.2zM18 6c-.55 0-1-.45-1-1s.45-1 1-1 1 .45 1 1-.45 1-1 1z"
            url="https://www.instagram.com/tonguy_platforms"
          />
          <SocialLink
            platform="Facebook"
            icon="M22 12c0-5.52-4.48-10-10-10S2 6.48 2 12c0 4.99 3.65 9.12 8.43 9.87V14.8h-2.9v-2.8h2.9V9.8c0-2.84 1.74-4.38 4.27-4.38 1.22 0 2.27.09 2.57.13v2.79h-1.66c-1.31 0-1.56.62-1.56 1.53V12h3.12l-.5 2.8h-2.62v7.07C18.35 21.12 22 16.99 22 12z"
            url="https://www.facebook.com/tonguyplatforms"
          />
          <SocialLink
            platform="X"
            icon="M22.46 6c-.88.39-1.83.65-2.82.77 1.01-.61 1.79-1.57 2.16-2.72-.95.56-2.01.97-3.13 1.19-.9-.96-2.18-1.56-3.6-1.56-2.72 0-4.93 2.21-4.93 4.93 0 .39.04.77.12 1.13-4.1-.2-7.73-2.17-10.16-5.14-.42.72-.66 1.56-.66 2.46 0 1.71.87 3.22 2.19 4.1-.8-.02-1.55-.25-2.2-.6v.06c0 2.39 1.7 4.38 3.95 4.83-.41.11-.85.17-1.3.17-.32 0-.63-.03-.93-.09.63 1.96 2.44 3.39 4.59 3.43-1.69 1.32-3.82 2.11-6.15 2.11-.4 0-.79-.02-1.18-.07 2.18 1.39 4.76 2.21 7.54 2.21 9.05 0 14-7.49 14-14.07 0-.22-.01-.43-.01-.65.96-.69 1.79-1.55 2.45-2.52z"
            url="https://twitter.com/tonguyplatforms"
          />
          <SocialLink
            platform="WeChat"
            icon="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1.5 14.5c-.83 0-1.5-.67-1.5-1.5s.67-1.5 1.5-1.5 1.5.67 1.5 1.5-.67 1.5-1.5 1.5zm3-3c-.83 0-1.5-.67-1.5-1.5s.67-1.5 1.5-1.5 1.5.67 1.5 1.5-.67 1.5-1.5 1.5z" // Generic chat icon, as specific WeChat icon is not standard in Lucide/FontAwesome.
            url="#" // Placeholder, replace with actual WeChat link if available
          />
          <SocialLink
            platform="WhatsApp"
            icon="M12 2C6.48 2 2 6.48 2 12c0 2.2.73 4.23 1.97 5.86L2 22l4.14-1.97C7.77 21.27 9.8 22 12 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm-1.5 14.5c-.83 0-1.5-.67-1.5-1.5s.67-1.5 1.5-1.5 1.5.67 1.5 1.5-.67 1.5-1.5 1.5zm3-3c-.83 0-1.5-.67-1.5-1.5s.67-1.5 1.5-1.5 1.5.67 1.5 1.5-.67 1.5-1.5 1.5z" // Generic chat icon, as specific WhatsApp icon is not standard in Lucide/FontAwesome.
            url="https://wa.me/yourwhatsappnumber" // Replace with actual WhatsApp link
          />
        </div>
      </section>

      {/* Footer */}
      <footer className="w-full max-w-6xl text-center text-gray-500 text-sm py-4">
        &copy; {new Date().getFullYear()} Tonguy Platforms. All rights reserved.
      </footer>
    </div>
  );
};

// Project Widget Component
const ProjectWidget = ({ title, description, link, imageUrl }) => {
  return (
    <div className="bg-gradient-to-br from-sky-50 to-sky-100 p-6 rounded-xl shadow-md hover:shadow-xl transition-all duration-300 transform hover:-translate-y-1">
      <img
        src={imageUrl}
        alt={title}
        className="w-full h-40 object-cover rounded-lg mb-4 shadow-sm"
        onError={(e) => {
          e.target.onerror = null;
          e.target.src = "https://placehold.co/400x250/E0E7FF/4338CA?text=Project"; // Fallback
        }}
      />
      <h3 className="text-xl font-bold text-sky-700 mb-2">{title}</h3>
      <p className="text-gray-700 text-sm mb-4">{description}</p>
      {link && (
        <a
          href={link}
          target="_blank"
          rel="noopener noreferrer"
          className="inline-block bg-sky-600 text-white px-5 py-2 rounded-full text-sm font-semibold hover:bg-sky-700 transition-colors duration-300 shadow-md"
        >
          Learn More
        </a>
      )}
    </div>
  );
};

// Social Link Component
const SocialLink = ({ platform, icon, url }) => {
  return (
    <a
      href={url}
      target="_blank"
      rel="noopener noreferrer"
      className="flex items-center justify-center p-3 rounded-full bg-sky-500 text-white shadow-md hover:bg-sky-600 transition-colors duration-300 transform hover:scale-105"
      aria-label={platform}
    >
      <svg className="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
        <path d={icon} />
      </svg>
      <span className="sr-only">{platform}</span> {/* For accessibility */}
    </a>
  );
};

export default App;
